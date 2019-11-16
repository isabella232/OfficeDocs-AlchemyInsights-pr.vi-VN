---
title: Thiếu quy trình làm việc không thể kích hoạt
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "36753818"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="495eb-102">Thiếu quy trình làm việc không thể kích hoạt</span><span class="sxs-lookup"><span data-stu-id="495eb-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="495eb-103">Trong bộ sưu tập trang web Microsoft SharePoint, bạn không thể thêm một công việc tái sử dụng toàn cầu (chẳng hạn như "phê duyệt-SharePoint 2010") vào một danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="495eb-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="495eb-104">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="495eb-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="495eb-105">Mở trang web gốc của bộ sưu tập trang web trong SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="495eb-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="495eb-106">Trong **trang web đối tượng**, chọn **luồng**công việc.</span><span class="sxs-lookup"><span data-stu-id="495eb-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="495eb-107">Trong phần **mới** của ruy băng **quy** trình, chọn công **việc tái**sử dụng.</span><span class="sxs-lookup"><span data-stu-id="495eb-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="495eb-108">Trên biểu mẫu **tạo luồng công việc tái** sử dụng, hãy nhập tên \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="495eb-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="495eb-109">Đối với **loại nền tảng**, bấm **SharePoint 2010 luồng công việc**, và sau đó bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="495eb-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="495eb-110">Trong phần **lưu** của ruy băng **luồng công việc** , chọn **xuất bản**.</span><span class="sxs-lookup"><span data-stu-id="495eb-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="495eb-111">Trong phần **quản lý** của Ribbon **luồng công việc** , chọn **xuất bản toàn cầu**.</span><span class="sxs-lookup"><span data-stu-id="495eb-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="495eb-112">Trong hộp thoại xác nhận xuất hiện, chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="495eb-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="495eb-113">Trong một trình duyệt web, xác định vị trí trang web gốc của bộ sưu tập trang web, và sau đó truy cập các **tính năng thu thập**trang web **thiết lập** \> trang web.</span><span class="sxs-lookup"><span data-stu-id="495eb-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="495eb-114">Sau đó, chuyển đổi tính năng **luồng** công việc:</span><span class="sxs-lookup"><span data-stu-id="495eb-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="495eb-115">· Nếu tính năng được *kích hoạt* , bấm vô hiệu hóa **,** và sau đó bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="495eb-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="495eb-116">· Nếu tính năng bị *hủy* **kích hoạt**, hãy nhấp vào bật.</span><span class="sxs-lookup"><span data-stu-id="495eb-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="495eb-117">Để biết thêm thông tin, vui lòng tham khảo [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)sau đây.</span><span class="sxs-lookup"><span data-stu-id="495eb-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

