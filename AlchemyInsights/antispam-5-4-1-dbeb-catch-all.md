---
title: AntiSpam 5.4.1 DBEB Catch-tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964377"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Khắc phục sự cố phân phối cho mã lỗi 550 5.4.1 truy cập từ chối chuyển tiếp

Sự cố này xảy ra khi [kiểm tra xem địa chỉ email có hợp lệ để ngăn chặn bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) khi nhập mạng Office 365. Hãy thử các mục sau:

1. Xác định xem sự cố dành riêng cho toàn bộ miền hoặc địa chỉ email duy nhất:
    - Toàn bộ miền: đôi khi miền cần được đồng bộ hoá; thử [đặt miền sang nội bộ và sau đó trở lại uỷ quyền](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
     - Địa chỉ email đơn: đôi khi địa chỉ cần được đồng bộ hoá; thay đổi địa chỉ proxy SMTP và sau đó thay đổi nó trở lại có thể giúp.
2. Xác định xem sự cố cụ thể cho một nhóm hoặc thư mục công cộng. Đối với một số loại đối tượng, các đối tượng có thể cần phải được tạo theo cách thủ công trong Azure Active Directory.

Nếu bạn cần thêm sự giúp đỡ, vui lòng mở một vé hỗ trợ và chỉ định phạm vi của vấn đề (includidng loại đối tượng bạn đang gửi đến) để chúng tôi có thể hỗ trợ bạn tốt hơn.