---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717347"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Khắc phục các sự cố chuyển phát email cho mã lỗi 5.7.23

Xác minh bản ghi SPF DNS cho tên miền của bạn tại một trình kiểm tra bản ghi SPF hoặc DNS công khai trên web.

Xác minh rằng thông báo gửi đi không được xác định là thư rác theo Microsoft và định tuyến thông qua [Hồ bơi chuyển giao rủi ro cao](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). Thư trong hồ bơi chuyển phát cao rủi ro sẽ không vượt qua kiểm tra SPF và do đó sẽ không được chấp nhận bởi tổ chức email đích.

Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với người quản trị máy chủ thư mà bạn đang tìm cách gửi email. Hãy lưu ý đến lỗi bên ngoài chi tiết sẵn dùng trong thư bị trả lại. Hỗ trợ của Microsoft có thể không thể hỗ trợ thêm nữa.
