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
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972738"
---
# <a name="troubleshoot-prt-issue"></a>Khắc phục sự cố PRT

Đối với bất kỳ thiết bị nào để hoàn tất quá trình xác thực, thiết bị phải được đăng ký đầy đủ và ở trạng thái tốt và có thể nhận được Mã thông báo Làm mới Chính (PRT).

Quy trình đăng ký liên kết Azure AD kết hợp yêu cầu các thiết bị nằm trên mạng công ty. VPN cũng hoạt động hơn VPN nhưng có một số lời nói trước cho điều đó. Chúng tôi đã nghe thấy các khách hàng cần hỗ trợ khắc phục sự cố cho quy trình đăng ký kết hợp Azure AD tham gia trong trường hợp làm việc từ xa. Dưới đây là phân tích về những gì đang xảy ra 'ở trong thành phố' trong quá trình đăng ký.

**Môi trường xác thực đám mây (sử dụng đồng bộ băm mật khẩu Azure AD hoặc xác thực thông qua)**

Dòng đăng ký này còn được gọi là "Kết nối đồng bộ".

1. Windows 10 sẽ phát hiện một bản ghi SCP khi người dùng đăng nhập vào thiết bị.
    1. Trước tiên, thiết bị tìm cách truy xuất thông tin đối tượng thuê từ SCP phía máy khách trong sổ đăng ký [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Để biết thêm thông tin, hãy xem tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Nếu không thành công, thiết bị sẽ liên lạc với Active Directory tại chỗ (AD) để lấy thông tin đối tượng thuê từ Điểm Kết nối Dịch vụ (SCP). Để xác minh SCP, vui lòng tham khảo tài [liệu này.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Chúng tôi khuyên bạn nên bật SCP trong AD và chỉ sử dụng SCP phía máy khách cho xác thực ban đầu.

2. Windows 10 liên lạc với Azure AD trong ngữ cảnh hệ thống để xác thực chính mình với Azure AD. Bạn có thể xác minh xem thiết bị có thể truy nhập tài nguyên Microsoft theo tài khoản hệ thống không bằng cách sử dụng script Kiểm tra Khả năng kết nối Đăng ký Thiết bị.

3. Windows 10 tạo ra một chứng chỉ tự ký và lưu trữ nó bên dưới đối tượng máy tính trong AD tại chỗ. Tính năng này yêu cầu liên quan đến Bộ điều khiển Miền.

4. Một đối tượng thiết bị có chứng chỉ sẽ được đồng bộ hóa với Azure AD thông qua Azure AD Kết nối. Chu kỳ đồng bộ là cách 30 phút một lần theo mặc định nhưng tùy thuộc vào cấu hình của Azure AD Kết nối. Để biết thêm thông tin, vui lòng tham khảo tài [liệu này.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. Ở giai đoạn này, bạn có thể thấy thiết bị chủ đề ở trạng thái "Đang chờ xử lý" trong Thiết bị của Cổng thông tin Azure.

6. Tại lần đăng nhập người dùng tiếp theo vào Windows 10, quá trình đăng ký sẽ được hoàn tất. 

> [!NOTE]
> Nếu bạn đang sử dụng VPN và quy trình đăng nhập logoff sẽ chấm dứt kết nối miền, bạn có thể kích hoạt đăng ký theo cách thủ công:
 1. Cấp phép /tham gia cục bộ trên lời nhắc quản trị hoặc từ xa thông qua PSExec vào PC của bạn. Ví dụ: PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Để biết thêm chi tiết về các sự cố Gia nhập Kết hợp, hãy xem Khắc [phục sự cố thiết bị](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
