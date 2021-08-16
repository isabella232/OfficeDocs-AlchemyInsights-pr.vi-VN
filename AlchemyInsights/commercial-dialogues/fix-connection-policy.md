---
title: Khắc phục chính sách kết nối
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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988234"
---
# <a name="fix-connection-policy"></a>Khắc phục chính sách kết nối

Email đã được đánh dấu an toàn và được chuyển đến hộp thư đến của người dùng vì địa chỉ IP gửi đã được đánh dấu an toàn trong chính sách Bộ lọc Kết nối. Để xem lại chính sách, hãy làm như sau:

1. Đi đến Trung [tâm Tuân Office 365 Security & Sau](https://go.microsoft.com/fwlink/p/?linkid=2077143)đó, đi đến Chính sách Quản lý mối đe dọa Chống thư   >    >  [rác](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Trên tab **Tùy chỉnh,** chọn chính sách **Bộ lọc kết nối**, sau đó chọn Chỉnh sửa chính **sách**.
3. Xem lại danh **sách IP Cho** phép. Xem liệu **danh Két sắt Tài liệu được** bật chưa.

    > [!NOTE]
    > Microsoft đăng ký các nguồn người gửi tin cậy của bên thứ ba. Nếu **Két sắt được** bật, những người gửi đáng tin cậy này sẽ không bị đánh dấu nhầm là thư rác. Tôi khuyên bạn nên chọn tùy chọn này, vì tùy chọn này sẽ làm giảm số lượng dương giả (thư tốt được phân loại là thư rác) mà bạn nhận được.
