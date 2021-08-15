---
title: Bạn cần đánh dấu miền hoặc danh sách người gửi email là an toàn?
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
- "9002921"
- "5673"
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025632"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Bạn cần đánh dấu miền hoặc danh sách người gửi email là an toàn?

- Chúng tôi **khuyên bạn không** nên dùng danh sách người gửi an toàn vì nó mở ra cho tổ chức của bạn thành cuộc tấn công thư rác, lừa đảo qua mạng và giả mạo.
- Tuy nhiên, nếu có yêu cầu kinh doanh, chúng tôi **khuyên bạn nên sử** dụng Quy tắc Flow Thư **[cho](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** điều này. Hướng dẫn của chúng tôi đảm bảo xác thực người gửi (xác nhận rằng miền gửi không bị giả mạo). **Lưu** ý : Chúng tôi khuyên bạn không nên quản lý tình trang phủ nhận sai bằng cách sử dụng danh sách người gửi an toàn, vì ngoại lệ cho việc lọc thư rác có thể mở tổ chức của bạn bị tấn công bảo mật. Nếu (những) người dùng của bạn nhận được thư được đánh dấu không đúng là thư rác hoặc email rác, vui lòng Báo cáo **[thư và tệp tới Microsoft.](https://protection.office.com/reportsubmission)**
- Két sắt Bạn nên tránh người gửi trong Outlook, Danh sách người  gửi được cho phép hoặc danh sách miền được cho phép trong các chính sách chống thư rác vì người gửi bỏ qua tất cả thư rác, giả mạo và bảo vệ lừa đảo và xác thực người gửi (SPF, DKIM, DMARC). Phương pháp này là phương pháp tốt nhất để chỉ dùng cho kiểm tra tạm thời.
- Có thể thực hiện xác thực cho một đánh giá Antispam được bỏ qua một email nhất định bằng cách kiểm tra thông tin thư "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), xem Tiêu đề thư chống thư **[rác.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Vì Microsoft muốn duy trì bảo mật cho khách hàng của [chúng](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)tôi theo mặc định, một số đối tượng thuê sẽ không được áp dụng cho phần mềm xấu và lừa đảo qua mạng với mức độ tin cậy cao. Những thay thế này bao gồm: o Danh sách người gửi được cho phép hoặc danh sách tên miền được cho phép (chính sách chống thư rác) o Outlook Két sắt Danh sách Cho phép IP (lọc kết nối) 
- Ghi đè duy nhất cho phép thư lừa đảo qua mạng có độ tin cậy cao để bỏ qua lọc là một Exchange tắc dòng thư (còn được gọi là quy tắc truyền tải). Để sử dụng quy tắc dòng thư để bỏ qua lọc, hãy xem Sử dụng quy tắc dòng thư để thiết lập mức tin cậy là thư **[rác (SCL) trong thư.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**