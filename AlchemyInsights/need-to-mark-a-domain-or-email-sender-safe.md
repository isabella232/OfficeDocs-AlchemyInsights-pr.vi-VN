---
title: Bạn cần đánh dấu tên miền hoặc người gửi email an toàn?
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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792154"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Bạn cần đánh dấu tên miền hoặc người gửi email an toàn?

- Sử dụng **danh sách người gửi an toàn không được đề** xuất vì nó mở ra tổ chức của bạn để thư rác, phish và các cuộc tấn công giả mạo.
- Tuy nhiên, nếu có một yêu cầu kinh doanh, chúng tôi **khuyên bạn nên** sử dụng các **[quy tắc dòng thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** cho điều này. Hướng dẫn của chúng tôi đảm bảo xác thực người gửi (xác nhận tên miền gửi không được spoofed). **Lưu ý**: chúng tôi không khuyên bạn nên quản lý tích cực false bằng cách sử dụng danh sách người gửi an toàn, vì ngoại lệ để lọc thư rác có thể mở tổ chức của bạn để bảo mật các cuộc tấn công. Nếu người dùng của bạn nhận được thư không đúng được đánh dấu là thư rác hoặc email rác, vui lòng **[báo cáo các thư và tệp vào Microsoft](https://protection.office.com/reportsubmission)**.
- Người gửi an toàn trong Outlook, danh sách người gửi được cho phép hoặc danh sách miền trong chính sách chống thư rác **sẽ bị tránh** vì người gửi bỏ qua tất cả các thư rác, spoof và bảo vệ bằng chữ và xác thực người gửi (SPF, DKIM, dMarc). Phương pháp này chỉ được sử dụng tốt nhất để kiểm tra tạm thời.
