---
title: Khắc phục chính sách Đối tượng thuê (thay thế hành động)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326819"
---
# <a name="fix-tenant-policy-action-override"></a>Khắc phục chính sách Đối tượng thuê (thay thế hành động)

Một trong những chính sách chống thư rác của bạn đã ảnh hưởng đến thư này. Để xem lại chính sách, hãy thực hiện các bước sau đây:

1. Trong cổng thông tin Bộ bảo vệ Microsoft 365 , đi đến Chính sách Cộng tác qua Email & Chính sách & Chính sách mối đe dọa Quy tắc Chính sách Chống thư <https://security.microsoft.com/>  \>  \>  \>  rác trong **phần Chính** sách.

   Để truy nhập trực tiếp vào **trang Chính sách chống thư rác,** hãy sử dụng <https://security.microsoft.com/antispam> .

2. Trên trang **Chính** sách chống thư rác, hãy chọn chính sách  bằng cách bấm  vào tên của chính sách **(** Loại là Chính sách chống thư rác tùy chỉnh hoặc Tên là Chính sách gửi thư đến Chống Thư rác **(Mặc định)).**
3. Trong hộp bật lên chi tiết xuất hiện, hãy chọn **Chỉnh sửa hành** động trong phần **Hành** động.
4. Trong phần Hành động **thư,** xem lại các bản pháp cho Thư  rác **,** Thư rác với độ tin cậy **cao,** Lừa đảo qua mạng và Lừa đảo qua mạng với độ tin cậy cao để xem liệu có bất kỳ giá trị nào sau đây được chọn không:
   - **Thêm dấu X đầu trang**
   - **Mở sẵn dòng chủ đề bằng văn bản**
   - **Chuyển hướng thư đến địa chỉ email**
   - **Xóa thư**
   - **Không hành động**

   Có thể cài đặt Tiêu chuẩn **được áp dụng cho** tất cả các Exchange Online Protection khách hàng đã ảnh hưởng đến thư.

Để biết thêm thông tin, hãy [xem Cấu hình chính sách chống thư rác trong EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
