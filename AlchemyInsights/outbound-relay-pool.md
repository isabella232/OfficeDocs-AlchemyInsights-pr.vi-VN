---
title: Nhóm chuyển tiếp đi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883153"
---
# <a name="outbound-relay-pool"></a>Nhóm chuyển tiếp đi

Microsoft đang thực hiện một số thay đổi đối với cấu hình để chuyển tiếp hoặc chuyển tiếp email thông qua Microsoft 365. Thư trong một số kịch bản nhất định được chuyển tiếp hoặc chuyển tiếp thông qua Microsoft 365 dụng một nhóm chuyển tiếp đặc biệt. Thư được gửi bằng cách dùng nhóm chuyển tiếp có thể dẫn đến thư mục thư rác của người nhận. Để biết thêm thông tin, hãy [xem Nhóm chuyển phát đi](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Để tránh kịch bản sử dụng nhóm chuyển tiếp, hãy đảm bảo rằng các thư chuyển tiếp/chuyển tiếp đáp ứng một trong các tiêu chí sau đây:

- Người gửi đi là tên miền được chấp nhận của đối tượng thuê.
- Khung Chính sách Người gửi (SPF) đi qua khi thư đến Microsoft 365.
- Thư được Xác định bởi DomainKeys (DKIM) trên miền người gửi P2 đi qua khi thư đến Microsoft 365.
 
Những thư đáp ứng các tiêu chí trên sẽ không được chuyển tiếp qua nhóm chuyển tiếp.

Nếu bản ghi MX cho tên miền của bạn được trỏ tới một máy chủ bên thứ ba hoặc tại chỗ, hãy sử dụng bộ lọc nâng cao để đảm bảo xác thực SPF chính xác cho email đến và tránh gửi email qua vùng chuyển tiếp.

**Làm thế nào để chúng tôi biết chúng tôi bị ảnh hưởng bởi nhóm chuyển tiếp?**

Nếu email chuyển tiếp hoặc chuyển tiếp sử dụng một trong các tiêu chí ở trên, thư sẽ không được chuyển tiếp thông qua nhóm chuyển tiếp. Tuy nhiên, nếu thư được gửi thông qua một nhóm chuyển tiếp, IP của máy chủ thư đi nằm trong phạm vi 40.95.0.0/16 và tên máy chủ thư đi bao gồm **rly** trong tên.

