---
title: Tôi nhận được quyền truy nhập có điều kiện với thiết bị tuân thủ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037082"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Tôi nhận được quyền truy nhập có điều kiện với thiết bị tuân thủ

**Công cụ được đề xuất cao**

- [Công cụ bộ giải quyết đăng ký thiết bị](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -công cụ toàn diện giúp khắc phục sự cố đăng ký thiết bị phổ biến nhất.
- [Script kết nối đăng ký thiết bị kiểm tra](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -công cụ được sử dụng để đảm bảo rằng thiết bị có thể truy nhập các điểm cuối đăng ký thiết bị bên dưới tài khoản hệ thống.
- [Kịch bản dọn dẹp thiết bị AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -một công cụ được sử dụng để tìm kiếm và quản lý các thiết bị cũ trong môi trường của bạn.

Dưới đây là một số lý do thông thường mà quyền truy nhập có điều kiện có thể không cho thiết bị tuân thủ hoặc tại sao người dùng của bạn có thể nhận được **bạn không thể đến đó từ thư ở đây** trong một yêu cầu đăng nhập vào một nguồn tài nguyên tổ chức.

1. **Thiết bị không có trong trạng thái thiết bị bắt buộc với MDM**:

Xác thực rằng thiết bị được đăng ký với một nhà cung cấp MDM được phê duyệt như InTune và được *đánh dấu là tuân thủ*. Để biết thêm thông tin về InTune, hãy xem [tài liệu](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)này. Để hiểu rõ hơn về việc tuân thủ thiết bị và InTune, hãy xem mục [sử dụng chính sách tuân thủ để đặt quy tắc cho các thiết bị mà bạn quản lý bằng InTune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Nếu bạn đang gặp sự cố đăng ký một thiết bị bằng InTune, hãy tìm chi tiết về khắc phục sự cố [trong việc khắc phục sự cố đăng ký thiết bị trong Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Để được hỗ trợ thêm InTune, hãy tạo một yêu cầu hỗ trợ. Để thực hiện việc này, hãy truy nhập [trang hỗ trợ và trợ giúp InTune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Thiết bị không được gia nhập vào mạng tổ chức**:

Để truy nhập vào các tài nguyên tổ chức, thiết bị phải được kết nối với mạng của tổ chức, thông qua kết nối trực tiếp hoặc mạng riêng ảo (VPN) và cũng đã tham gia vào các thư mục tại chỗ hoặc Azure Active Directory. Để gia nhập thiết bị làm việc với mạng của tổ chức, hãy xem [gia nhập thiết bị công việc của bạn với mạng của tổ chức bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Để đăng ký thiết bị cá nhân/BYOD, hãy xem [mục đăng ký thiết bị cá nhân của bạn trên mạng của tổ chức của bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Để xác thực thiết bị đã gia nhập mạng, bạn có thể làm theo các bước cho thiết bị đã đăng ký [ở đây](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) hoặc các thiết bị làm việc [tại đây](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Để phạm vi vấn đề về kết nối mạng của tổ chức, hãy làm theo hướng dẫn dưới đây:

    1. Đăng nhập vào Windows bằng tài khoản cơ quan hoặc trường học của bạn, ví dụ: alain@contoso.com.
    2. Kết nối với mạng của tổ chức của bạn thông qua VPN hoặc truy nhập Direct.
    3. Sau khi bạn đã kết nối, hãy nhấn **phím logo Windows + L** để khóa thiết bị của bạn.
    4. Mở khóa thiết bị của bạn bằng tài khoản cơ quan hoặc trường học của bạn, rồi thử truy nhập vào ứng dụng hoặc dịch vụ có vấn đề.

Nếu bạn thấy thông báo lỗi **sau đây bạn không thể** gặp phải, vấn đề có thể ở những nơi khác.

3. **Hệ điều hành không được hỗ trợ**:

Đảm bảo rằng bạn đang chạy phiên bản được hỗ trợ của hệ điều hành, bao gồm:

- **Máy khách Windows**: Windows 7 trở lên

- **Windows Server**: windows Server 2008 R2 hoặc phiên sau này

- **MacOS**: MacOS X trở lên

- **Android và iOS**: Phiên bản mới nhất của hệ điều hành Android và iOS dành cho thiết bị di động

4. **Trình duyệt web không được hỗ trợ**:

Vui lòng tìm các trình duyệt được hỗ trợ bên dưới. Đối với hỗ trợ Chrome với Windows 1703 hoặc phiên bản mới hơn, phần mở rộng tài khoản Windows 10 là bắt buộc. Đối với cạnh 85 +, người dùng cần phải đăng nhập đúng thông tin tuân thủ theo thiết bị. Để biết thêm chi tiết, hãy xem mục [ở đây](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, InTune được quản lý trình duyệt, Safari
- **Android**: **Microsoft Edge**: InTune được quản lý trình duyệt, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Tìm hiểu thêm thông tin về việc **bạn không thể nhận được** thông báo và các bước khắc phục sự cố [ở đây](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
