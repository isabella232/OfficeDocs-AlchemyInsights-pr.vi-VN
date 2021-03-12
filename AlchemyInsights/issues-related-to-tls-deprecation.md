---
title: Không thể gửi/nhận email đến/từ Office 365 vì của TLS 1,0 và TLS 1,1 đã ngừng phân tích
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747111"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Không thể gửi/nhận email đến/từ Office 365 vì của TLS 1,0 và TLS 1,1 đã ngừng phân tích

Khi được xác nhận bởi Trung tâm thông báo Post MC229914, TLS 1,0 và TLS 1,1 việc phản đối bắt đầu thực thi các điểm cuối dòng thư Exchange Online. Soon Office 365 sẽ không còn chấp nhận kết nối email TLS 1,0 và TLS 1,1 từ các nguồn bên ngoài. Ngoài ra, Exchange Online sẽ không bao giờ sử dụng TLS 1,0 hoặc 1,1 để gửi email đi. Nếu bạn đang gặp phải sự cố vì 1,0 hoặc 1,1 không phân hủy, bạn có thể gặp một trong các lỗi sau đây-

- Người gửi đang nhận được NDR Bounce Back-' 421 kết nối 4.4.2 bị bỏ do SocketError '
- Lỗi trong trình xem xếp hàng của máy chủ tại chỗ đang gửi email đến sĩ quan 365-' 421 4.4.2 kết nối bị bỏ do SocketError '
- Lỗi trong gửi [Nhật ký giao thức](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) đường kết nối trên máy chủ gửi email đến Office 365-TLS không thành công với SocketError lỗi
- Lỗi trong Nhật ký gửi hoặc nhận giao thức đường kết nối-' 451 5.7.3 phải phát hành lệnh STARTTLS đầu tiên '

Nếu bạn gặp bất kỳ lỗi nào ở trên, hãy đảm bảo rằng máy chủ đang gửi hoặc nhận email đã bật TLS 1,2 bằng cách kiểm tra các khóa đăng ký sau đây-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ máy khách] **"DisabledByDefault" = DWORD: 00000000 "bật" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ máy chủ] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Nếu bạn thực hiện bất kỳ thay đổi nào trong các phím đăng ký ở trên để bật TLS 1,2, hãy khởi động lại máy chủ để các thay đổi có hiệu lực. Ngoài ra, hãy đảm bảo bạn đã cài đặt các bản cập nhật Windows và Exchange mới nhất.

Để biết thêm thông tin, hãy xem:

- [Hướng dẫn về Exchange Server TLS, phần 1: chuẩn bị sẵn sàng cho TLS 1,2-cộng đồng kỹ thuật của Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Phần hướng dẫn của Exchange Server TLS 2: bật TLS 1,2 và xác định khách hàng không sử dụng CNTT-cộng đồng kỹ thuật của Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Hiểu rõ tình huống email nếu không thể thỏa thuận Phiên bản TLS với Exchange Online-Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
