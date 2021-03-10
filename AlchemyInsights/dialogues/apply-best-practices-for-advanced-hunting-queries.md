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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="c471b-102">Áp dụng các phương pháp tốt nhất cho truy vấn săn bắn nâng cao</span><span class="sxs-lookup"><span data-stu-id="c471b-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="c471b-103">Để có được kết quả nhanh hơn và để tránh thời chờ trong khi chạy truy vấn phức tạp, hãy áp dụng những cách thực hành tốt nhất này:</span><span class="sxs-lookup"><span data-stu-id="c471b-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="c471b-104">Khi thử các truy vấn mới, luôn sử dụng giới hạn, để tránh việc tập kết quả rất lớn.</span><span class="sxs-lookup"><span data-stu-id="c471b-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="c471b-105">Ngoài ra, hãy sử dụng `count` để thực hiện đánh giá ban đầu về kích cỡ của tập kết quả.</span><span class="sxs-lookup"><span data-stu-id="c471b-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="c471b-106">Sử dụng bộ lọc thời gian trước tiên.</span><span class="sxs-lookup"><span data-stu-id="c471b-106">Use time filters first.</span></span> <span data-ttu-id="c471b-107">Lý tưởng nhất, giới hạn truy vấn của bạn thành bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="c471b-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="c471b-108">Trong phần bắt đầu của một truy vấn, ngay sau khi lọc thời gian, hãy thêm bộ lọc dự kiến sẽ loại bỏ hầu hết dữ liệu.</span><span class="sxs-lookup"><span data-stu-id="c471b-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="c471b-109">Khi tìm kiếm thẻ đầy đủ, hãy dùng `has` toán tử chứ không phải `contains` .</span><span class="sxs-lookup"><span data-stu-id="c471b-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="c471b-110">Chạy tìm kiếm trên một cột cụ thể chứ không phải trên tất cả các cột.</span><span class="sxs-lookup"><span data-stu-id="c471b-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="c471b-111">Khi tham gia bảng, trước tiên, hãy xác định bảng với các hàng ít hơn.</span><span class="sxs-lookup"><span data-stu-id="c471b-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="c471b-112">`project` chỉ các cột cần thiết từ các bảng mà bạn đã gia nhập.</span><span class="sxs-lookup"><span data-stu-id="c471b-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="c471b-113">Để tìm hiểu thêm, hãy xem các cách [thực hành tốt nhất của truy vấn săn bắn nâng cao](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="c471b-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
