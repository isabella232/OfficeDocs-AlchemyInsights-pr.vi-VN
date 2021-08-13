---
title: Tôi bị Quyền truy nhập có Điều kiện chặn với thiết bị kết nối theo miền
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
ms.openlocfilehash: f0d092dfbc805b1e4fa7d26803227118b39ecacca9fa330bb5de8458d4aa0f57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950318"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Tôi bị Quyền truy nhập có Điều kiện chặn với thiết bị kết nối theo miền

**Công cụ được Đề xuất Cao**

[Công cụ Trình khắc phục sự cố Đăng ký](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) Thiết bị - Công cụ giúp khắc phục các sự cố đăng ký thiết bị phổ biến nhất.

[Script Kiểm tra Kết nối Đăng ký Thiết](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) bị - Tập lệnh giúp đảm bảo rằng một thiết bị có thể truy nhập các điểm cuối Đăng ký Thiết bị theo tài khoản hệ thống.

[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - Tập lệnh cho phép bạn tìm kiếm và quản lý các thiết bị cũ trong môi trường của mình.

Dưới đây là một số lý do phổ biến về việc truy nhập có điều kiện có thể gây ra lỗi cho thiết bị đã liên kết miền (Azure AD Hỗn hợp).

1. **Không có Azure AD PRT** trên thiết bị - Bạn cần phải đảm bảo rằng thiết bị có Mã thông báo Làm mới Chính của Azure AD (PRT). Để biết thêm thông tin về PRT, hãy xem tài [liệu này](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Để xác minh xem bạn có Azure AD PRT chưa, bạn có thể chạy lệnh trên thiết bị, rồi xác minh xem `dsregcmd/status` "AzureAdPrt" có phải là "CÓ".

Nếu "AzureAdPrt" là "NO", hãy kiểm tra như sau:

- Liệu bạn có môi trường liên kết với **AD FS hay không** và không thể liên kết với các mạng nội bộ của người dùng: Trong trường hợp này, hãy đảm bảo rằng các điểm cuối "tên người dùng" của bạn đều có thể truy nhập từ mạng nội bộ mở rộng. Nếu AD FS của bạn ẩn VPN, hãy đảm bảo rằng người dùng kết nối với VPN và đăng nhập lại vào thiết bị. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Việc TPM của** thiết bị có bị lỗi không thể xác thực thiết bị hay không: Đánh dấu vào "tpm.msc" để xem trạng thái của TPM có phải là "Sẵn sàng". Nếu không, hãy `dsregcmd/leave` chạy và cho phép thiết bị tham gia lại vào Azure AD. Sau đó, thử lại. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Bạn đang sử dụng nhà cung cấp định danh bên thứ 3 không hỗ trợ giao WS-Trust bên thứ 3.** Như đã mô tả trong tài liệu của chúng tôi, các thiết bị kết hợp Azure AD kết hợp không thể hoạt động trong trường hợp này. Vui lòng làm việc với nhà cung cấp định danh của bạn để được hỗ trợ.

2. Người dùng đang sử dụng trình duyệt Chrome khi không có Tài khoản **Windows 10** hoặc phần mở rộng Office Chrome không tự động sử dụng PRT trên các thiết bị kết hợp AAD hoặc kết **hợp-AAD** kết hợp: Điều này dẫn đến sự cố dẫn đến lỗi của mọi chính sách Truy nhập Có điều kiện dựa trên thiết bị, kèm theo thông báo lỗi "Thiết bị chưa đăng ký" được hiển thị. Để sử dụng đúng trình duyệt Chrome, bạn phải cài đặt "Tài khoản Windows 10" hoặc "phần mở rộng Office cho trình duyệt Chrome của người dùng" thông qua SCCM hoặc Intune. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Nếu không thể đẩy tiện ích bổ trợ từ xa, hãy thông báo cho người dùng để cài đặt thủ công một trong những phần mở rộng trên để truy nhập vào các ứng dụng dựa trên thiết bị Có điều kiện. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Thiết bị đã kết hợp đúng cách với Azure AD nhưng đã vô tình bị xóa hoặc bị vô hiệu hóa, do thay đổi đồng bộ trong Azure AD Kết nối hoặc từ cổng thông tin **Azure:** Nếu điều này xảy ra, đối tượng thiết bị sẽ không còn được nhận dạng là thiết bị nối đầy đủ ngay cả khi trạng thái "AzureAdJoined" và "PRT" sẽ hiển thị là hợp lệ trên thiết bị.

Để khắc phục sự cố này, `dsregcmd/leave` hãy chạy trên các thiết bị bị ảnh hưởng và cho phép họ gia nhập lại Azure AD. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Nếu thiết bị của bạn đang sử dụng bản cập nhật Windows 10, phiên bản 1809 với VPN/Cloud Proxy và thấy các sự cố về trạng thái "AzureAdPrt" hoặc bất kỳ ứng dụng nào có sự cố SSO (outlook không kết nối đến hộp thư ngay cả khi bạn đã có PRT), hãy đảm bảo rằng bạn có bản sửa lỗi [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) hoặc bản cập nhật tích lũy Tháng Tư [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) để ngăn chặn các lỗi PRT trên các máy đó.

















