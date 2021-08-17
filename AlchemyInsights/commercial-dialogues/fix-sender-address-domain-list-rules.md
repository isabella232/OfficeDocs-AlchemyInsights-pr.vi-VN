---
title: Khắc phục các Địa chỉ Người gửi tắc danh sách Tên miền/Tên miền
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
ms.openlocfilehash: db8b921fc84f42b6cef1138dca9ad433e648e0a2f10e80927bd5b0222bfeae3b
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896133"
---
# <a name="fix-sender-addressdomain-list-rules"></a>Khắc phục các Địa chỉ Người gửi tắc danh sách Tên miền/Tên miền

Một trong những chính sách chống thư rác của bạn đã ảnh hưởng đến thư này. Người gửi thư đã được tìm thấy trong danh sách Cho phép hoặc Chặn. Để xem lại chính sách, hãy thực hiện các bước sau đây:

1. Trong cổng thông tin Bộ bảo vệ Microsoft 365 , đi đến Chính sách Cộng tác qua Email & các chính sách & chính sách Mối đe dọa Quy tắc Chống thư <https://security.microsoft.com/>  \>  \>  \>  rác trong **phần Chính** sách.

   Để truy nhập trực tiếp vào **trang Chính sách chống thư rác,** hãy sử dụng <https://security.microsoft.com/antispam> .

2. Trên trang **Chính** sách chống thư rác, hãy chọn chính sách  bằng cách bấm  vào tên của chính sách **(** Loại là Chính sách chống thư rác tùy chỉnh hoặc Tên là Chính sách gửi thư đến Chống Thư rác **(Mặc định)).**
3. Trong cửa sổ bật lên  chi tiết xuất hiện, chọn Chỉnh sửa người gửi và tên miền bị chặn và cho phép trong mục Người gửi và tên miền được cho phép và **bị** chặn.
4. Trong phần **Cho phép,** hãy xem lại người gửi và tên miền bằng cách bấm Quản **lý người \<nn\> gửi** **hoặc Cho phép tên miền.**

Để biết thêm thông tin, hãy [xem Cấu hình chính sách chống thư rác trong EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
