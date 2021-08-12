---
title: Người dùng của bạn có nhận được email độc hại không
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929219"
---
# <a name="did-your-users-receive-malicious-email"></a>Người dùng của bạn có nhận được email độc hại không?

- Bây giờ bạn có thể báo cáo email độc hại tới Microsoft bằng cách sử dụng Các [bản gửi của Người quản trị trong Trung tâm & Tuân thủ.](https://sip.protection.office.com/reportsubmission)

Các thư được gửi trong các [bản gửi của người quản trị](https://sip.protection.office.com/reportsubmission) sẽ được quét và các kết quả sau đây được hiển thị trong hộp bật **lên** chi tiết:

- Nếu xảy ra lỗi trong xác thực email của người gửi tại thời điểm chuyển phát.
- Thông tin về bất kỳ lượt truy cập chính sách nào có thể làm ảnh hưởng hoặc ghi đè bản án của thư.
- Kết quả giải kích hoạt hiện tại để xem liệu các URL hoặc tệp có trong thư có độc hại hay không.
- Phản hồi từ điểm số

Nếu tìm thấy ghi đè, việc chỉnh lại có thể hoàn tất trong vài phút. Nếu không có sự cố trong xác thực email hoặc nếu việc chuyển phát không bị ảnh hưởng bởi việc ghi đè thì có thể mất tối đa một ngày để nhận phản hồi từ các điểm số.

Nếu bạn không đồng ý với bản quyết định cuối cùng về thư, URL hoặc tệp (bị chặn và không bị chặn), hãy gửi lại thư sau một ngày để thử lại. Khả năng cao là quyết định sẽ thay đổi sau khi gửi lại thư.

Đồng thời, bạn có thể loại bỏ email độc hại khỏi hộp thư đến của người dùng bằng cách làm theo các hướng dẫn [trong bài viết này.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Khách hàng có Bộ bảo vệ Microsoft dành cho doanh Office 365 có thể:
    - sử dụng [Trình khám phá Mối đe dọa để Tìm và Xóa email Đáng ngờ](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [sử Két sắt Nối kết để chặn quyền truy nhập](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) vào URL độc hại
    - theo dõi người dùng đã bấm và truy nhập URL độc hại: Xem [URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)lừa đảo qua mạng và bấm vào dữ liệu xác định  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - bắt đầu [Điều tra Tự động theo cách thủ công](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Bạn cũng có thể bảo vệ chống lại các tệp và URL độc hại bằng cách làm theo các hướng dẫn trong mục [Bảo vệ khỏi các URL và tệp độc hại.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)