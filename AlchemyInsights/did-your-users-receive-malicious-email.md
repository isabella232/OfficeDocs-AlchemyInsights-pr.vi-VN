---
title: Người dùng của bạn có nhận được email độc hại hay không
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291814"
---
# <a name="did-your-users-receive-malicious-email"></a>Người dùng của bạn có nhận được email độc hại không?

- Giờ đây, bạn có thể báo cáo email độc hại với Microsoft bằng cách sử dụng trình [gửi người quản trị trong Trung tâm tuân thủ & bảo mật](https://sip.protection.office.com/reportsubmission).

Các thư được gửi trong [đệ trình quản trị](https://sip.protection.office.com/reportsubmission) được quét và các kết quả sau đây được hiển thị trong **thông tin chi tiết** :

- Nếu đã xảy ra lỗi trong xác thực email của người gửi tại thời điểm chuyển phát.
- Thông tin về bất kỳ số truy cập chính sách nào có thể bị ảnh hưởng hoặc ghi đè lên bản án của thư.
- Kết quả phát nổ hiện tại để xem các URL hoặc tệp chứa trong thư bị độc hại hay không.
- Phản hồi từ học sinh lớp

Nếu đã tìm thấy ghi đè, thì Rescan sẽ hoàn thành trong vài phút. Nếu không có vấn đề gì trong xác thực email hoặc nếu quá trình chuyển không bị ảnh hưởng bởi dấu ghi đè, thì phản hồi từ các học sinh học có thể mất tới một ngày.

Nếu bạn không đồng ý với bản án cuối cùng trên thư, URL hoặc tệp (bị chặn vs không bị chặn), hãy gửi tin nhắn lại sau một ngày để thu hồi lại. Cơ hội cao là bản án sẽ thay đổi sau khi gửi lại thư.

Trong khi đó, bạn có thể loại bỏ email độc hại khỏi các hộp thư của người dùng bằng cách làm theo các hướng dẫn trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Khách hàng với Microsoft Defender cho Office 365 có thể:
    - sử dụng [Threat Explorer để tìm và xóa email đáng ngờ](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [sử dụng liên kết an toàn để chặn quyền truy nhập](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) vào URL độc hại
    - theo dõi người dùng đã bấm và truy nhập URL độc hại: [xem URL giả mạo và bấm vào bản án dữ liệu](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)  &  [Get-urltrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - [bắt đầu một điều tra tự động](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office) theo cách thủ công

Bạn cũng có thể bảo vệ chống lại các tệp và URL độc hại bằng cách theo dõi các hướng dẫn trong việc [bảo vệ khỏi URL và tệp độc hại](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).