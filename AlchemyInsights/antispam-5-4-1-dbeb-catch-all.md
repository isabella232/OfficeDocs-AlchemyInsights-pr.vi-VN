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
ms.openlocfilehash: ad0f4c691a5e06306dbb408f4d66a4e00609e4d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43707933"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Khắc phục sự cố phân phối cho mã lỗi 550 5.4.1 truy cập từ chối chuyển tiếp

Sự cố này xảy ra khi [kiểm tra xem địa chỉ email có hợp lệ để ngăn chặn bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) khi nhập mạng Microsoft. Hãy thử các mục sau:

1. Xác định xem sự cố dành riêng cho toàn bộ miền hoặc địa chỉ email duy nhất:
    - Toàn bộ miền: đôi khi miền cần được đồng bộ hoá; thử [đặt miền sang nội bộ và sau đó trở lại uỷ quyền](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Địa chỉ email đơn: đôi khi địa chỉ cần được đồng bộ hoá; thay đổi địa chỉ proxy SMTP và sau đó thay đổi nó trở lại có thể giúp.
2. Xác định xem sự cố cụ thể cho một nhóm hoặc thư mục công cộng. Đối với một số loại đối tượng, các đối tượng có thể cần phải được tạo theo cách thủ công trong Azure Active Directory.

Nếu bạn cần thêm trợ giúp, vui lòng mở một vé ủng và chỉ định phạm vi của vấn đề (bao gồm loại đối tượng bạn đang gửi đến) để chúng tôi có thể hỗ trợ bạn tốt hơn.