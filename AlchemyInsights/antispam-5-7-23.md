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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682356"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Khắc phục sự cố gửi email cho mã lỗi 5.7.23

Xác minh bản ghi SPF DNS cho miền của bạn tại một công khai có SPF hoặc kiểm tra bản ghi DNS trên web.

Xác minh rằng thư đi không được xác định là thư rác của Office 365 và chuyển qua vùng [phân phối rủi ro cao](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). Thư trong vùng phân phối rủi ro cao sẽ không vượt qua kiểm tra SPF và do đó sẽ không được chấp nhận bởi tổ chức email đích.

Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với quản trị viên của máy chủ thư mà bạn đang cố gắng gửi email. Hãy lưu ý các lỗi bên ngoài chi tiết có sẵn trong thư trả lại.  Hỗ trợ Office 365 không thể hỗ trợ thêm.