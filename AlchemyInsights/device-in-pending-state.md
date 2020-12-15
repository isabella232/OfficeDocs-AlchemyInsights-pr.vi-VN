---
title: Thiết bị trong trạng thái đang chờ xử lý
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679997"
---
# <a name="device-in-pending-state"></a>Thiết bị trong trạng thái đang chờ xử lý

**OLSync**

1. Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, vui lòng đảm bảo rằng bạn đã xem xét việc [giới thiệu về quản lý thiết bị trong Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) sẽ hướng dẫn bạn về cách tải các thiết bị dưới phần điều khiển của Azure AD.
2. Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và ghi lại chúng vào InTune, bạn sẽ cần phải đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tại chỗ trước tiên.
3. Đảm bảo bạn được phép thực hiện các hoạt động trong Azure AD và quảng cáo tại cơ sở. Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị. Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ của bạn, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).

Quy trình tham gia đăng ký kết hợp Azure AD sẽ yêu cầu thiết bị trên mạng công ty. Nó cũng hoạt động trên VPN nhưng có một số cẩn thận với điều đó. Chúng tôi đã nghe những khách hàng cần trợ giúp khắc phục sự cố về quy trình đăng ký kết hợp Azure.

**Môi trường xác thực đám mây (sử dụng tính năng đồng bộ hóa băm mật khẩu Azure AD hoặc chuyển qua)**

Dòng đăng ký này còn được gọi là "đồng bộ gia nhập".

Dưới đây là một sự cố về những điều sẽ xảy ra trong quá trình đăng ký:

1. Bản ghi điểm kết nối dịch vụ phát hiện Windows 10 (SCP) khi người dùng đăng nhập vào thiết bị.

    1. Trước tiên, thiết bị cố gắng truy xuất thông tin đối tượng thuê từ SCP bên máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Nếu không thành công, thiết bị liên lạc với Active Directory tại chỗ để nhận thông tin về đối tượng thuê từ SCP. Để xác nhận SCP, hãy tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)này.

    > [!NOTE]
    > Chúng tôi khuyên bạn nên bật SCP trong Active Directory và chỉ sử dụng SCP-Side cho máy khách để xác thực ban đầu.

2. Windows 10 sẽ cố gắng liên lạc với Azure AD bên dưới ngữ cảnh hệ thống để xác thực chính nó với Azure AD.

    Bạn có thể xác nhận liệu thiết bị có thể truy nhập tài nguyên Microsoft bên dưới tài khoản hệ thống bằng cách sử dụng [script kết nối đăng ký thiết bị kiểm tra](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 tạo chứng chỉ tự ký và lưu trữ nó bên dưới đối tượng máy tính trong Active Directory tại chỗ. Điều này yêu cầu phải có đường ngắm cho bộ điều khiển tên miền.

4. Đối tượng thiết bị có chứng chỉ được đồng bộ hóa với Azure AD thông qua Azure AD Connect. Chu kỳ đồng bộ là mỗi 30 phút theo mặc định, nhưng tùy thuộc vào cấu hình của Azure AD Connect. Để biết thêm thông tin, hãy tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)này.

5. Ở giai đoạn này, bạn sẽ có thể nhìn thấy thiết bị chủ đề trong trạng thái "**đang chờ**" bên dưới thanh thiết bị của Azure Portal.

6. Tại mục đăng nhập của người dùng tiếp theo vào Windows 10, việc đăng ký sẽ được hoàn thành.

    > [!NOTE]
    > Nếu bạn đang ở trên VPN và đăng xuất/đăng nhập chấm dứt khả năng kết nối tên miền, bạn có thể kích hoạt việc đăng ký theo cách thủ công. Để thực hiện điều đó:
    >
    > Phát hành `dsregcmd /join` lời nhắc người quản trị cục bộ hoặc từ xa qua PSExec sang PC của bạn.
    >
    > Ví dụ: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Đối với các sự cố phổ biến với đăng ký thiết bị Azure Active Directory, hãy xem [thiết bị câu hỏi thường gặp](https://docs.microsoft.com/azure/active-directory/devices/faq).
