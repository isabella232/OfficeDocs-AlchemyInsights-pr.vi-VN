---
title: Bạn cần đánh dấu một tên miền hoặc người gửi email an toàn?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281241"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Bạn cần đánh dấu một tên miền hoặc người gửi email an toàn?

- **Không nên sử dụng danh sách người gửi an toàn** vì nó mở ra tổ chức của bạn để thư rác, lừa, và giả mạo tấn công.
- Tuy nhiên, nếu có yêu cầu kinh doanh, chúng tôi **khuyên bạn nên** sử dụng **[quy tắc luồng thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** cho điều này. Hướng dẫn của chúng tôi đảm bảo xác thực người gửi (kiểm tra miền gửi không bị spoofed). **Lưu ý**: chúng tôi không khuyên bạn nên quản lý sai tích cực bằng cách sử dụng danh sách người gửi an toàn, vì ngoại lệ để lọc thư rác có thể mở tổ chức của bạn để tấn công bảo mật. Nếu (các) người dùng của bạn nhận được thư không đúng đánh dấu là spam hoặc email rác, vui lòng **[báo cáo tin nhắn và tệp cho Microsoft](https://protection.office.com/reportsubmission)**.
- Người gửi an toàn trong Outlook, được phép gửi danh sách hoặc danh sách cho phép tên miền trong chính sách chống thư rác **nên tránh** bởi vì người gửi bỏ qua tất cả thư rác, giả mạo và bảo vệ phish và xác thực gửi (SPF, DKIM, dMarc). Phương pháp này được sử dụng tốt nhất để kiểm tra tạm thời chỉ.
