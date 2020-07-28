---
title: Biểu đồ hiển thị số lượng bản ghi khác nhau trong lưới
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439957"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="0c99b-102">Biểu đồ hiển thị số lượng bản ghi khác nhau trong lưới</span><span class="sxs-lookup"><span data-stu-id="0c99b-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="0c99b-103">**Triệu chứng**</span><span class="sxs-lookup"><span data-stu-id="0c99b-103">**Symptom**</span></span>

<span data-ttu-id="0c99b-104">Đối với biểu đồ trên trang bảng điều khiển, khi bạn nhấp vào biểu đồ "..." và nhấp vào "xem bản ghi", bạn điều hướng đến trang lưới để xem tất cả các bản ghi. Đôi khi, số lượng hồ sơ thay đổi.</span><span class="sxs-lookup"><span data-stu-id="0c99b-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="0c99b-105">**Gây ra**</span><span class="sxs-lookup"><span data-stu-id="0c99b-105">**Cause**</span></span>

<span data-ttu-id="0c99b-106">Điều này là do sự khác biệt giữa lượt xem giữa biểu đồ trên trang bảng điều khiển gốc và biểu đồ trên trang chủ lưới.</span><span class="sxs-lookup"><span data-stu-id="0c99b-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="0c99b-107">**Giải pháp**</span><span class="sxs-lookup"><span data-stu-id="0c99b-107">**Solution**</span></span>

1. <span data-ttu-id="0c99b-108">Kiểm tra xem từ trang gốc và xem trong lưới để xem nếu họ là khác nhau.</span><span class="sxs-lookup"><span data-stu-id="0c99b-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="0c99b-109">Thay đổi giao diện trong lưới để phù hợp với giao diện trong trang gốc.</span><span class="sxs-lookup"><span data-stu-id="0c99b-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="0c99b-110">Nếu không tìm thấy đúng xem, thường nó có nghĩa là xem không được kích hoạt trong công cụ thiết kế ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="0c99b-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="0c99b-111">Đi tới công cụ thiết kế ứng dụng của ứng dụng riêng, chọn thực thể và quan điểm của nó, kiểm tra xem bạn muốn bật, lưu, xuất bản và đóng.</span><span class="sxs-lookup"><span data-stu-id="0c99b-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="0c99b-112">Làm mới trang.</span><span class="sxs-lookup"><span data-stu-id="0c99b-112">Refresh the page.</span></span>