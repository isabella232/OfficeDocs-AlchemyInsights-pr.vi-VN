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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888428"
---
# <a name="fix-connection-policy"></a>Khắc phục chính sách kết nối

Email đã được đánh dấu an toàn và được chuyển đến Hộp thư đến của người dùng vì địa chỉ IP nguồn đã được đánh dấu là an toàn trong chính sách bộ lọc kết nối mặc định. Để xem lại chính sách, hãy thực hiện các bước sau đây:

1. Trong cổng thông tin Bộ bảo vệ Microsoft 365 , đi đến Chính sách Cộng tác qua Email & các chính sách & chính sách Mối đe dọa Quy tắc Chống thư <https://security.microsoft.com/>  \>  \>  \>  rác trong **phần Chính** sách.

   Để truy nhập trực tiếp vào **trang Chính sách chống thư rác,** hãy sử dụng <https://security.microsoft.com/antispam> .

2. Trên trang **Chính sách chống thư rác,** hãy chọn chính sách có tên Chính sách bộ lọc kết nối **(Mặc định)** bằng cách bấm vào tên của chính sách.

3. Trong hộp bật lên chi tiết xuất hiện, bấm Chỉnh **sửa chính sách bộ lọc kết** nối trong phần Lọc **kết** nối.

4. Xem lại các mục nhập trong mục Luôn cho phép thư **gửi từ** các địa chỉ IP hoặc dải địa chỉ sau và xem liệu Bật danh sách an toàn **có** được chọn hay không.

   > [!NOTE]
   > Microsoft đăng ký các nguồn người gửi tin cậy của bên thứ ba. Nếu danh sách an toàn được bật, những người gửi đáng tin cậy này sẽ không bị đánh dấu nhầm là thư rác. Chúng tôi khuyên bạn nên chọn tùy chọn này, vì tùy chọn này sẽ làm giảm số lượng dương giả (thư tốt được phân loại là thư rác) mà bạn nhận được.

Để biết thêm thông tin, hãy xem [Cấu hình lọc kết nối](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy).
