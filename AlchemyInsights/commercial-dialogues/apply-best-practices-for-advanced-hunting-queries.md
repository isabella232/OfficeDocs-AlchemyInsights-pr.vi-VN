---
title: Áp dụng các biện pháp tốt nhất cho truy vấn bảo vệ nâng cao
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930155"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Áp dụng các biện pháp tốt nhất cho truy vấn bảo vệ nâng cao

Để có được kết quả nhanh hơn và tránh tình trạng hết thời gian chờ trong khi chạy truy vấn phức tạp, hãy áp dụng các biện pháp tốt nhất sau:

- Khi thử truy vấn mới, hãy luôn sử dụng giới hạn để tránh nhận các tập kết quả cực lớn. Ngoài ra, sử `count` dụng để đánh giá ban đầu kích cỡ của tập kết quả.
- Trước tiên, hãy sử dụng bộ lọc thời gian. Tốt nhất là hãy giới hạn truy vấn của bạn trong bảy ngày.
- In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.
- Khi bạn tìm kiếm mã thông báo đầy đủ, hãy sử dụng `has` toán tử thay vì `contains` .
- Chạy tìm kiếm trên một cột cụ thể chứ không phải trên tất cả các cột.
- Khi tham gia các bảng, trước tiên, hãy chỉ định bảng có ít hàng hơn.
- `project` chỉ các cột cần thiết từ các bảng mà bạn đã nối.

Để tìm hiểu thêm, hãy xem cách [thực hành tốt nhất cho truy vấn săn bắn nâng cao](https://go.microsoft.com/fwlink/?linkid=2144812).
