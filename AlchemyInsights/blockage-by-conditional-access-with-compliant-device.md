---
title: Tôi bị Quyền truy cập có Điều kiện chặn với thiết bị tương thích
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019170"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Tôi bị Quyền truy cập có Điều kiện chặn với thiết bị tương thích

**Công cụ được Đề xuất Cao**

- [Công cụ Khắc phục sự cố Đăng ký Thiết](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) bị - Một công cụ toàn diện giúp khắc phục các sự cố đăng ký thiết bị phổ biến nhất.
- [Script Kiểm tra Kết nối Đăng ký Thiết](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) bị - Một công cụ được sử dụng để đảm bảo thiết bị có thể truy nhập các điểm cuối Đăng ký Thiết bị theo tài khoản hệ thống.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - Một công cụ được sử dụng để tìm kiếm và quản lý các thiết bị cũ trong môi trường của bạn.

Dưới đây là một số lý do phổ biến về việc Truy nhập có Điều  kiện có thể không thành công đối với một thiết bị tuân thủ hoặc tại sao người dùng của bạn có thể nhận được Bạn không thể nhận được thông báo từ đây trong khi yêu cầu đăng nhập vào tài nguyên của tổ chức.

1. **Thiết bị không ở trạng thái thiết bị bắt buộc với MDM:**

Xác thực rằng thiết bị được đăng ký với nhà cung cấp MDM được phê duyệt như Intune và được đánh *dấu là đã tuân thủ.* Để biết thêm thông tin về Intune, hãy xem tài [liệu này](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Để hiểu rõ hơn về tuân thủ thiết bị và Intune, hãy xem mục sử dụng chính sách tuân thủ để đặt quy tắc cho thiết bị [bạn quản lý với Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Nếu bạn đang gặp sự cố khi đăng ký thiết bị với Intune, hãy tìm chi tiết khắc phục sự cố tại [Khắc phục sự cố đăng ký thiết bị trong Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Để được hỗ trợ thêm về Intune, hãy tạo một yêu cầu hỗ trợ. Để làm vậy, hãy truy cập [trang Trợ giúp và Hỗ trợ của Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Thiết bị không được tham gia mạng tổ chức**:

Để truy nhập vào các tài nguyên tổ chức, thiết bị phải được kết nối với mạng của tổ chức, thông qua kết nối trực tiếp hoặc mạng riêng ảo (VPN), cũng tham gia vào mạng tại chỗ hoặc tại Azure Active Directory. Để tham gia một thiết bị công ty vào mạng tổ chức, hãy xem [Gia nhập thiết bị cơ quan của bạn vào mạng của tổ chức bạn](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Để đăng ký thiết bị cá nhân/BYOD, hãy xem [Đăng ký thiết bị cá nhân của bạn trên mạng của tổ chức bạn.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Để xác thực xem thiết bị đã tham gia mạng hay chưa, bạn có thể làm theo các bước dành cho thiết bị đã đăng ký tại [đây hoặc](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) các thiết bị làm việc [tại đây](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Để đưa sự cố vào kết nối mạng tổ chức, hãy làm theo các hướng dẫn dưới đây:

    1. Đăng nhập vào tài Windows bằng tài khoản cơ quan hoặc trường học của bạn, ví dụ: alain@contoso.com.
    2. Kết nối mạng của tổ chức bạn thông qua VPN hoặc DirectAccess.
    3. Sau khi bạn kết nối, hãy **nhấn Windows logo+L để** khóa thiết bị của bạn.
    4. Mở khóa thiết bị bằng tài khoản cơ quan hoặc trường học của bạn, rồi thử truy nhập lại vào ứng dụng hoặc dịch vụ có sự cố.

Nếu bạn thấy thông báo **Lỗi Bạn không thể đến đó từ đây một lần nữa** thì sự cố có thể xảy ra ở nơi khác.

3. **Hệ điều hành không được hỗ trợ:**

Đảm bảo rằng bạn đang chạy phiên bản hệ điều hành được hỗ trợ, bao gồm:

- **Windows Client**: Windows 7 trở lên

- **Windows Server**: Windows Server 2008 R2 trở lên

- **macOS**: macOS X trở lên

- **Android và iOS**: Phiên bản hệ điều hành mới nhất của Android và iOS dành cho thiết bị di động

4. **Trình duyệt web không được hỗ trợ:**

Vui lòng tìm các trình duyệt được hỗ trợ bên dưới. Để hỗ trợ Chrome với Windows 1703 trở lên, cần có phần mở rộng Windows 10 khoản người dùng. Đối với Edge 85+, người dùng cần đăng nhập để thông tin tuân thủ thiết bị đúng cách. Để biết thêm chi tiết, hãy xem [tại đây.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Trình duyệt được Quản lý của Intune, Safari
- **Android**: **Microsoft Edge**: Trình duyệt được Quản lý của Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Tìm thêm thông tin về thông **báo Bạn không thể nhận được thông báo đó và** các bước khắc phục sự cố ở [đây](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
