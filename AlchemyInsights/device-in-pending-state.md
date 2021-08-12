---
title: Thiết bị đang chờ xử lý
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914025"
---
# <a name="device-in-pending-state"></a>Thiết bị đang chờ xử lý

**Điều kiện tiên quyết:**

1. Nếu bạn thiết lập đăng ký thiết bị lần đầu tiên, vui lòng đảm bảo rằng bạn đã xem lại Giới thiệu về quản lý thiết bị trong [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) sẽ hướng dẫn bạn cách nhận thiết bị dưới quyền kiểm soát của Azure AD.
2. Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và đăng ký thiết bị [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) vào Intune, bạn sẽ cần phải đảm bảo rằng bạn đã đặt cấu hình [cho Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và tiến hành cấp phép trước.
3. Đảm bảo bạn được phép thực hiện các thao tác trong Azure AD và AD tại chỗ. Chỉ người quản trị toàn cầu trong Azure AD mới có thể quản lý cài đặt cho đăng ký thiết bị. Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).

Quy trình đăng ký liên kết Azure AD kết hợp yêu cầu các thiết bị phải nằm trên mạng công ty. VPN cũng hoạt động hơn VPN nhưng có một số lời nói trước cho điều đó. Chúng tôi đã lắng nghe khách hàng cần hỗ trợ khắc phục sự cố cho quy trình đăng ký kết hợp Azure AD trong các trường hợp làm việc từ xa.

**Môi trường xác thực đám mây (sử dụng đồng bộ băm mật khẩu Azure AD hoặc xác thực thông qua)**

Dòng đăng ký này còn được gọi là "Kết nối đồng bộ".

Dưới đây là phân tích về những điều xảy ra trong quá trình đăng ký:

1. Windows 10 phát hiện bản ghi Điểm Kết nối Dịch vụ (SCP) khi người dùng đăng nhập vào thiết bị.

    1. Trước tiên, thiết bị tìm cách truy xuất thông tin đối tượng thuê từ SCP phía máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Nếu không thành công, thiết bị sẽ liên lạc với Active Directory tại cơ sở để nhận thông tin đối tượng thuê từ SCP. Để xác minh SCP, hãy tham khảo tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Chúng tôi khuyên bạn nên bật SCP trong Active Directory và chỉ sử dụng SCP phía máy khách để xác thực ban đầu.

2. Windows 10 liên lạc với Azure AD trong ngữ cảnh hệ thống để xác thực chính mình với Azure AD.

    Bạn có thể xác minh xem thiết bị có thể truy nhập tài nguyên Microsoft theo tài khoản hệ thống không bằng cách sử dụng script [Kiểm tra Khả năng kết nối Đăng ký Thiết bị.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 tạo chứng chỉ tự ký và lưu trữ chứng chỉ đó bên dưới đối tượng máy tính trong Active Directory tại chỗ. Tính năng này yêu cầu liên quan đến Bộ điều khiển Miền.

4. Đối tượng thiết bị có chứng chỉ được đồng bộ hóa với Azure AD thông qua Azure AD Kết nối. Chu kỳ đồng bộ là cách 30 phút một lần theo mặc định nhưng tùy thuộc vào cấu hình của Azure AD Kết nối. Để biết thêm thông tin, hãy tham khảo tài [liệu này](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. Ở giai đoạn này, bạn có thể thấy thiết bị chủ đề ở trạng thái **"** Đang chờ xử lý " trong Thiết bị của Cổng thông tin Azure.

6. Tại lần đăng nhập người dùng tiếp theo vào Windows 10, quá trình đăng ký sẽ được hoàn tất.

    > [!NOTE]
    > Nếu bạn đang sử dụng VPN và logoff/login chấm dứt kết nối miền, bạn có thể kích hoạt đăng ký theo cách thủ công. Cách thực hiện:
    >
    > Cấp lời `dsregcmd /join` nhắc cục bộ trên lời nhắc người quản trị hoặc từ xa thông qua PSExec đến PC của bạn.
    >
    > Ví dụ: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Để biết các sự cố thường gặp với Azure Active Directory thiết bị, hãy xem Câu [hỏi thường gặp về thiết bị.](https://docs.microsoft.com/azure/active-directory/devices/faq)
