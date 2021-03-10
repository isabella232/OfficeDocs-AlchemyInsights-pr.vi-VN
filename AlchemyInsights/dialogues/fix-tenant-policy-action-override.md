---
title: Sửa chữa chính sách đối tượng thuê (ghi đè hành động)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695688"
---
# <a name="fix-tenant-policy-action-override"></a>Sửa chữa chính sách đối tượng thuê (ghi đè hành động)

Chính sách chống thư rác trong đối tượng thuê của bạn bị ảnh hưởng trong thư này. Để xem lại chính sách, hãy làm như sau:

1. Truy nhập [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), rồi đi tới chính sách chống thư rác về **quản lý mối đe dọa**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Kiểm tra xem **nguồn chính sách** cho biết như sau:  **Thêm-XHeader/Modifysubject/Redirect/Delete/No Action/Bcc Message**

    Nếu vậy, trên tab **tùy chỉnh** , hãy kiểm tra các thiết đặt của chính sách ảnh hưởng đến thư. Có thể các **thiết đặt tiêu chuẩn** được áp dụng cho tất cả các khách hàng bảo vệ Exchange Online đã ảnh hưởng đến thư.

Để biết thêm thông tin về cách cấu hình chính sách bộ lọc thư rác, hãy xem [cấu hình chính sách bộ lọc thư rác của bạn](https://go.microsoft.com/fwlink/?linkid=2101431).
