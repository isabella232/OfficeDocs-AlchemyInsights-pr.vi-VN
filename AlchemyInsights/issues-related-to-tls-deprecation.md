---
title: Không thể gửi/nhận email đến/Office 365 vì vô hiệu hóa TLS 1.0 và TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054928"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Không thể gửi/nhận email đến/Office 365 vì vô hiệu hóa TLS 1.0 và TLS 1.1

Như đã xác nhận bởi bài đăng trong trung tâm thông báo MC229914, việc bỏ dùng TLS 1.0 và TLS 1.1 bắt đầu thực thi cho Exchange Online điểm cuối dòng thư. Sắp Office 365 sẽ không còn chấp nhận kết nối email TLS 1.0 và TLS 1.1 từ các nguồn bên ngoài nữa. Ngoài ra, Exchange Online bao giờ sử dụng TLS 1.0 hoặc 1.1 để gửi email đi. Nếu bạn đang gặp phải sự cố do vô hiệu hóa TLS 1.0 hoặc 1.1, bạn có thể gặp phải một trong các lỗi sau đây-

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Lỗi trong Trình xem Hàng đợi của máy chủ Tại chỗ đang gửi email đến Officer 365- '421 4.4.2 Kết nối bị mất do SocketError'
- Lỗi trong nhật ký Giao [thức trình](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) kết nối Gửi trên máy chủ gửi email đến Office 365- Việc đàm phán TLS không thành công với lỗi SocketError
- Lỗi trong nhật ký giao thức bộ nối Gửi hoặc nhận - '451 5.7.3 Phải phát hành lệnh STARTTLS trước tiên'

Nếu bạn gặp bất kỳ lỗi nào trong số những lỗi trên, vui lòng đảm bảo máy chủ đang gửi hoặc nhận email đã bật TLS 1.2 bằng cách kiểm tra các khóa đăng ký sau đây-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Máy khách] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Nếu bạn thực hiện bất kỳ thay đổi nào trong khóa đăng ký bên trên để bật TLS 1.2, hãy khởi động lại máy chủ để thay đổi có hiệu lực. Ngoài ra, hãy đảm bảo bạn đã cài đặt bản cập Windows và bản cập Exchange mới nhất.

Để biết thêm thông tin, hãy xem:

- [Exchange Server Hướng dẫn TLS, phần 1: Chuẩn bị Sẵn sàng cho TLS 1.2 - Cộng đồng Kỹ thuật Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Hướng dẫn TLS Phần 2: Cho phép TLS 1.2 và Xác định Máy khách Không sử dụng TLS - Cộng đồng Kỹ thuật Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Hiểu rõ các kịch bản email nếu không thể đồng ý với các phiên bản TLS Exchange Online - Cộng đồng Kỹ thuật Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
