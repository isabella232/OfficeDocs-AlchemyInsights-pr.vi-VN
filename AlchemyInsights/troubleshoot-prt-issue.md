---
title: Khắc phục sự cố PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573906"
---
# <a name="troubleshoot-prt-issue"></a>Khắc phục sự cố PRT

Đối với bất kỳ thiết bị nào để hoàn tất việc nhận đã được xác thực, nó phải được đăng ký đầy đủ và trong trạng thái tốt và có thể thu được mã thông báo làm mới chính (PRT).

Quy trình tham gia đăng ký kết hợp Azure AD sẽ yêu cầu thiết bị trên mạng công ty. Nó cũng hoạt động trên VPN nhưng có một số cẩn thận với điều đó. Chúng tôi đã nghe những khách hàng cần trợ giúp khắc phục sự cố về quy trình đăng ký kết hợp Azure. Đây là một sự cố về những điều đang xảy ra ' dưới mui xe ' trong quá trình đăng ký.

**Môi trường xác thực đám mây (sử dụng tính năng đồng bộ hóa băm mật khẩu Azure AD hoặc chuyển qua)**

Dòng đăng ký này còn được gọi là "đồng bộ gia nhập".

1. Windows 10 phát hiện ra một bản ghi SCP khi người dùng đăng nhập vào thiết bị.
    1. Trước tiên, thiết bị cố gắng truy xuất thông tin đối tượng thuê từ SCP bên máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Để biết thêm thông tin, hãy xem [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)này.
    2. Nếu không thành công, thiết bị liên lạc với Active Directory tại cơ sở (quảng cáo) để nhận thông tin đối tượng thuê từ điểm kết nối dịch vụ (SCP). Để xác nhận SCP, vui lòng tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)này. 

> [!NOTE]
> Chúng tôi khuyên bạn nên bật SCP trong quảng cáo và chỉ sử dụng SCP bên máy khách để xác thực ban đầu.

2. Windows 10 sẽ cố gắng liên lạc với Azure AD bên dưới ngữ cảnh hệ thống để xác thực chính nó với Azure AD. Bạn có thể xác nhận liệu thiết bị có thể truy nhập tài nguyên Microsoft bên dưới tài khoản hệ thống bằng cách sử dụng script kết nối đăng ký thiết bị kiểm tra.

3. Windows 10 tạo chứng chỉ tự ký và lưu trữ nó bên dưới đối tượng máy tính trong quảng cáo tại cơ sở. Điều này yêu cầu phải có đường ngắm cho bộ điều khiển tên miền.

4. Đối tượng thiết bị có chứng chỉ được đồng bộ hóa với Azure AD thông qua Azure AD Connect. Chu kỳ đồng bộ là mỗi 30 phút theo mặc định, nhưng tùy thuộc vào cấu hình của Azure AD Connect. Để biết thêm thông tin, vui lòng tham khảo [tài liệu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)này.

5. Ở giai đoạn này, bạn sẽ có thể nhìn thấy thiết bị chủ đề trong trạng thái "đang chờ" bên dưới thanh thiết bị của Azure Portal.

6. Tại mục đăng nhập của người dùng tiếp theo vào Windows 10, việc đăng ký sẽ được hoàn thành. 

> [!NOTE]
> Nếu bạn đang ở trên VPN và quá trình đăng nhập kết thúc kết nối tên miền, bạn có thể kích hoạt theo cách thủ công:
 1. Phát hành hàm dsregcmd/join cục bộ trên lời nhắc quản trị hoặc từ xa qua PSExec đến PC của bạn. Ví dụ: PsExec-s \\ win10client01 CMD, dsregcmd/join

 2. Để biết thêm chi tiết về các vấn đề gia nhập kết hợp, hãy xem [khắc phục sự cố thiết bị](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
