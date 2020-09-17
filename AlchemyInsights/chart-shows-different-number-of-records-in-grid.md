---
title: Biểu đồ hiển thị số lượng bản ghi khác nhau trong lưới
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793780"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="4caf4-102">Biểu đồ hiển thị số lượng bản ghi khác nhau trong lưới</span><span class="sxs-lookup"><span data-stu-id="4caf4-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="4caf4-103">**Chứng**</span><span class="sxs-lookup"><span data-stu-id="4caf4-103">**Symptom**</span></span>

<span data-ttu-id="4caf4-104">Đối với biểu đồ trên trang bảng điều khiển, khi bạn bấm vào biểu đồ "..." và bấm vào "xem bản ghi", bạn dẫn hướng đến trang lưới để xem tất cả các bản ghi. Đôi khi, số lượng bản ghi thay đổi.</span><span class="sxs-lookup"><span data-stu-id="4caf4-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="4caf4-105">**Bởi**</span><span class="sxs-lookup"><span data-stu-id="4caf4-105">**Cause**</span></span>

<span data-ttu-id="4caf4-106">Điều này là do sự khác biệt giữa các dạng xem giữa biểu đồ trên trang bảng điều khiển ban đầu và biểu đồ trên trang chủ lưới.</span><span class="sxs-lookup"><span data-stu-id="4caf4-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="4caf4-107">**Nghiệm**</span><span class="sxs-lookup"><span data-stu-id="4caf4-107">**Solution**</span></span>

1. <span data-ttu-id="4caf4-108">Kiểm tra dạng xem từ trang gốc và dạng xem trong lưới để xem liệu chúng có khác hay không.</span><span class="sxs-lookup"><span data-stu-id="4caf4-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="4caf4-109">Thay đổi dạng xem trong lưới để khớp với dạng xem trong trang ban đầu.</span><span class="sxs-lookup"><span data-stu-id="4caf4-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="4caf4-110">Nếu không tìm thấy dạng xem chính xác, thông thường nó có nghĩa là dạng xem không được bật trong trình thiết kế ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="4caf4-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="4caf4-111">Đi tới trình thiết kế ứng dụng của ứng dụng cụ thể, chọn tổ chức và dạng xem của nó, kiểm tra xem bạn muốn bật, lưu, phát hành và đóng.</span><span class="sxs-lookup"><span data-stu-id="4caf4-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="4caf4-112">Làm mới trang.</span><span class="sxs-lookup"><span data-stu-id="4caf4-112">Refresh the page.</span></span>