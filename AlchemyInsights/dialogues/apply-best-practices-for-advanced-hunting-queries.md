---
title: Áp dụng các phương pháp tốt nhất cho truy vấn săn bắn nâng cao
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696078"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Áp dụng các phương pháp tốt nhất cho truy vấn săn bắn nâng cao

Để có được kết quả nhanh hơn và để tránh thời chờ trong khi chạy truy vấn phức tạp, hãy áp dụng những cách thực hành tốt nhất này:

- Khi thử các truy vấn mới, luôn sử dụng giới hạn, để tránh việc tập kết quả rất lớn. Ngoài ra, hãy sử dụng `count` để thực hiện đánh giá ban đầu về kích cỡ của tập kết quả.
- Sử dụng bộ lọc thời gian trước tiên. Lý tưởng nhất, giới hạn truy vấn của bạn thành bảy ngày.
- Trong phần bắt đầu của một truy vấn, ngay sau khi lọc thời gian, hãy thêm bộ lọc dự kiến sẽ loại bỏ hầu hết dữ liệu.
- Khi tìm kiếm thẻ đầy đủ, hãy dùng `has` toán tử chứ không phải `contains` .
- Chạy tìm kiếm trên một cột cụ thể chứ không phải trên tất cả các cột.
- Khi tham gia bảng, trước tiên, hãy xác định bảng với các hàng ít hơn.
- `project` chỉ các cột cần thiết từ các bảng mà bạn đã gia nhập.

Để tìm hiểu thêm, hãy xem các cách [thực hành tốt nhất của truy vấn săn bắn nâng cao](https://go.microsoft.com/fwlink/?linkid=2144812).
