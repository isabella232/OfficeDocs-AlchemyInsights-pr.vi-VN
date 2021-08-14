---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932191"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Khắc phục các vấn đề chuyển email cho mã lỗi 5.7.23

Xác nhận bản ghi DNS SPF cho tên miền của bạn tại bộ kiểm tra bản ghi SPF hoặc DNS công khai trên web.

Xác minh rằng thư đi không được Microsoft xác định là thư rác và được định tuyến thông qua Nhóm [Chuyển phát Rủi ro Cao.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Thư trong Nhóm Chuyển phát Rủi ro Cao sẽ không vượt qua kiểm tra SPF và do đó sẽ không được tổ chức email đích chấp nhận.

Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với người quản trị của máy chủ thư mà bạn đang tìm cách gửi email. Lưu ý về lỗi bên ngoài chi tiết có trong thông báo không gửi thư. Bộ trợ giúp của Microsoft có thể không hỗ trợ được thêm.
