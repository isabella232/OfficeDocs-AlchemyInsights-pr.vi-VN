---
title: Tôi nhận quyền truy nhập có điều kiện với thiết bị đã tham gia tên miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038108"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Tôi nhận quyền truy nhập có điều kiện với thiết bị đã tham gia tên miền

**Công cụ được đề xuất cao**

[Công cụ trình gỡ rối đăng ký thiết bị](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) -công cụ giúp khắc phục sự cố đăng ký thiết bị phổ biến nhất.

Trình [kiểm tra kết nối đăng ký thiết bị](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) -Script giúp đảm bảo rằng thiết bị có thể truy nhập các điểm cuối đăng ký thiết bị bên dưới tài khoản hệ thống.

[Kịch bản dọn dẹp thiết bị AZURE AD](https://github.com/mzmaili/AzureADDeviceCleanup) -tập lệnh cho phép bạn tìm kiếm và quản lý các thiết bị cũ trong môi trường của bạn.

Dưới đây là một số lý do phổ biến tại sao truy nhập có điều kiện có thể không phải là một thiết bị đã gia nhập một tên miền (kết hợp Azure AD).

1. **Không có AZURE AD PRT trên thiết bị** -bạn cần đảm bảo rằng thiết bị có mã thông báo làm mới của Azure AD (PRT). Để biết thêm thông tin về PRT, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)này.

Để xác nhận nếu bạn có Azure AD PRT, bạn có thể chạy `dsregcmd/status` lệnh trên thiết bị và xác nhận xem "AzureAdPrt" bằng "có".

Nếu "AzureAdPrt" là "không", hãy kiểm tra như sau:

- **Cho dù bạn có môi trường được liên kết với AD FS và không thể truy nhập được từ mạng nhà của người dùng của bạn**: trong trường hợp này, hãy đảm bảo rằng các điểm cuối "usernamemixed" của bạn có thể truy nhập từ Extranet. Nếu AD FS của bạn nằm phía sau một VPN, hãy đảm bảo rằng người dùng kết nối với VPN và đăng nhập lại vào thiết bị. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)này.

- **Cho dù thiết bị của TPM bị lỗi và do đó không thể xác thực thiết bị**: Hãy kiểm tra "TPM. msc" để xem trạng thái của TPM là "đã sẵn sàng". Nếu không, `dsregcmd/leave` hãy chạy và để thiết bị gia nhập lại AZURE AD. Sau đó, hãy thử lại. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)này.

- **Bạn đang sử dụng nhà cung cấp căn cước bên thứ 3, vốn không hỗ trợ giao thức WS-Trust**. Như được mô tả trong tài liệu của chúng tôi, kết hợp Azure AD được gia nhập vào các thiết bị không thể làm việc trong trường hợp này. Vui lòng làm việc với nhà cung cấp căn cước của bạn để được hỗ trợ.

2. **Người dùng đang sử dụng trình duyệt Chrome mà không có tài khoản Windows 10** hoặc **Chrome của Office sẽ không tự động sử dụng PRT trên thiết bị đã tham gia hoặc** kết hợp kết hợp-kết hợp với thiết bị được gia nhập: điều này sẽ dẫn đến sự thất bại của bất kỳ thông báo lỗi truy nhập có điều kiện dựa trên thiết bị nào được hiển thị. Để sử dụng trình duyệt Chrome chính xác, bạn phải cài đặt phần mở rộng "tài khoản Windows 10" hoặc "Office Extension với trình duyệt Chrome của người dùng" thông qua SCCM hoặc InTune. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)này.

Nếu bạn không thể đẩy phần mở rộng từ xa, hãy thông báo cho người dùng để cài đặt thủ công một trong các phần mở rộng để truy nhập vào các ứng dụng sau quyền truy nhập có điều kiện dựa trên thiết bị. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)này.

3. **Thiết bị được kết hợp đúng cách kết hợp AZURE AD đã gia nhập nhưng đã vô tình bị xóa hoặc tắt, do việc đồng bộ thay đổi trong AZURE AD Connect hoặc từ Azure Portal**: nếu điều này xảy ra, đối tượng thiết bị sẽ không còn được nhận diện là thiết bị được gia nhập đầy đủ, mặc dù trạng thái "AzureAdJoined" và

Để khắc phục sự cố này, `dsregcmd/leave` hãy chạy trên các thiết bị bị ảnh hưởng và để họ tái gia nhập AZURE AD. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)này.

> [!NOTE]
> Nếu các thiết bị của bạn đang ở trên Windows 10, 1809 Cập Nhật, với VPN/proxy proxy và xem các vấn đề với "AzureAdPrt" State hoặc ứng dụng bất kỳ với vấn đề SSO (Outlook không kết nối đến hộp thư ngay cả khi bạn đã có PRT), hãy đảm bảo bạn có bản vá này [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) hoặc bản Cập Nhật tích lũy tháng tư [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) để ngăn chặn các

















