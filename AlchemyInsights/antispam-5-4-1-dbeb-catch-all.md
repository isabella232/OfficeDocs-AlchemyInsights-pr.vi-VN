---
title: AntiSpam 5.4.1 \ Catch-tất cả
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821469"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Khắc phục các sự cố chuyển phát cho mã lỗi 550 5.4.1 Relay Access bị từ chối

Sự cố này xảy ra khi [kiểm tra để xem liệu một địa chỉ email có hiệu lực hợp lệ không để ngăn chặn](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) khi nhập mạng Microsoft. Hãy thử làm như sau:

1. Xác định xem vấn đề này là gì cụ thể đối với toàn bộ tên miền hoặc địa chỉ email duy nhất:
    - Toàn bộ tên miền: đôi khi tên miền cần được đồng bộ hóa; thử [đặt tên miền thành nội bộ và sau đó trở lại thẩm quyền](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Địa chỉ email đơn: đôi khi địa chỉ cần được đồng bộ hóa; thay đổi địa chỉ proxy SMTP và sau đó thay đổi nó lại có thể trợ giúp.
2. Xác định xem vấn đề này là gì cụ thể đối với một nhóm hoặc thư mục công cộng. Đối với một số loại đối tượng, các đối tượng có thể cần được tạo theo cách thủ công trong Azure Active Directory.

Nếu bạn cần thêm trợ giúp, vui lòng mở một vé hỗ trợ và xác định phạm vi vấn đề (bao gồm loại đối tượng mà bạn đang gửi đến) để chúng tôi có thể hỗ trợ bạn tốt hơn.