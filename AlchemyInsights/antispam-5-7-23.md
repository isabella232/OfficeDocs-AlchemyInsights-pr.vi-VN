---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506465"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Khắc phục sự cố gửi email cho mã lỗi 5.7.23

Xác minh bản ghi SPF DNS cho miền của bạn tại một công khai có SPF hoặc kiểm tra bản ghi DNS trên web.

Xác minh rằng thư đi không được xác định là thư rác của Microsoft và chuyển qua vùng [phân phối rủi ro cao](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Thư trong vùng phân phối rủi ro cao sẽ không vượt qua kiểm tra SPF và do đó sẽ không được chấp nhận bởi tổ chức email đích.

Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với quản trị viên của máy chủ thư mà bạn đang cố gắng gửi email. Hãy lưu ý các lỗi bên ngoài chi tiết có sẵn trong thư trả lại. Hỗ trợ của Microsoft không thể hỗ trợ thêm.
