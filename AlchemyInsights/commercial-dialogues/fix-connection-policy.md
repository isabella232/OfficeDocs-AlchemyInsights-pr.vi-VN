---
title: Sửa chính sách kết nối
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750595"
---
# <a name="fix-connection-policy"></a>Sửa chính sách kết nối

Email được đánh dấu an toàn và được gửi đến hộp thư đến của người dùng vì địa chỉ IP của việc gửi được đánh dấu an toàn trong chính sách bộ lọc kết nối. Để xem lại chính sách, hãy làm như sau:

1. Truy nhập [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), rồi đi tới chính sách chống thư rác về **quản lý mối đe dọa**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Trên tab **tùy chỉnh** , hãy chọn **chính sách bộ lọc kết nối**, rồi chọn **sửa chính sách**.
3. Xem lại danh sách **IP cho phép** . Xem **danh sách an toàn** được bật không.

    > [!NOTE]
    > Microsoft đăng ký sang nguồn bên thứ ba của người gửi tin cậy. Nếu đã bật **danh sách an toàn** , những người gửi tin cậy này không bị nhầm lẫn được đánh dấu là thư rác. Tôi khuyên bạn nên chọn tùy chọn này, vì nó sẽ giảm số lượng dương tính false (thư tốt được phân loại là thư rác) mà bạn nhận được.
