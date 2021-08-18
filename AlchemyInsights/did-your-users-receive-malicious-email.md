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
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326732"
---
# <a name="did-your-users-receive-malicious-email"></a>Người dùng của bạn có nhận được email độc hại không?

Bây giờ bạn có thể báo cáo email độc hại tới Microsoft bằng [cách sử dụng Gửi trong Bộ bảo vệ Microsoft 365 tin.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Các thư được gửi trong các [bản gửi của người quản trị](https://security.microsoft.com/reportsubmission?viewid=admin) sẽ được quét và các kết quả sau đây được hiển thị trong hộp bật lên chi tiết:

- Nếu xảy ra lỗi trong xác thực email của người gửi tại thời điểm chuyển phát.
- Thông tin về bất kỳ lượt truy cập chính sách nào có thể làm ảnh hưởng hoặc ghi đè bản án của thư.
- Kết quả giải kích hoạt hiện tại để xem liệu các URL hoặc tệp có trong thư có độc hại hay không.
- Phản hồi từ điểm số

Nếu tìm thấy ghi đè, việc chỉnh lại có thể hoàn tất trong vài phút. Nếu không có sự cố trong xác thực email hoặc nếu việc chuyển phát không bị ảnh hưởng bởi việc ghi đè thì có thể mất tối đa một ngày để nhận phản hồi từ các điểm số.

Nếu bạn không đồng ý với bản quyết định cuối cùng về thư, URL hoặc tệp (bị chặn và không bị chặn), hãy gửi lại thư sau một ngày để thử lại. Khả năng cao là quyết định sẽ thay đổi sau khi gửi lại thư.

Đồng thời, bạn có thể loại bỏ email độc hại khỏi hộp thư đến của người dùng bằng cách làm theo các hướng dẫn [trong bài viết này.](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)

- Khách hàng có Bộ bảo vệ Microsoft dành cho doanh Office 365 có thể:
  - Sử dụng [Trình khám phá Mối đe dọa để Tìm và Xóa email Đáng ngờ](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Sử dụng Két sắt nối kết để chặn quyền truy nhập](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) vào URL độc hại
  - Theo dõi người dùng đã bấm và truy nhập URL độc hại: Xem [URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)lừa đảo qua mạng và bấm vào dữ liệu xác định  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Bắt đầu [Điều tra Tự động theo cách thủ công](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Bạn cũng có thể bảo vệ chống lại các tệp và URL độc hại bằng cách làm theo các hướng dẫn trong mục [Bảo vệ khỏi các URL và tệp độc hại.](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)
