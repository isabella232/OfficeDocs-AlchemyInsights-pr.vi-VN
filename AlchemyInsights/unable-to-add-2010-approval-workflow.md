---
title: Không thể thêm 2010 phê duyệt luồng công việc
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582869"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="dd85d-102">Không thể thêm 2010 phê duyệt luồng công việc</span><span class="sxs-lookup"><span data-stu-id="dd85d-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="dd85d-103">Trong bộ sưu tập trang web Microsoft SharePoint, bạn không thể thêm một công việc tái sử dụng toàn cầu (chẳng hạn như "phê duyệt-SharePoint 2010") vào một danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="dd85d-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="dd85d-104">Để khắc phục sự cố này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="dd85d-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="dd85d-105">Mở trang web gốc của bộ sưu tập trang web trong SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="dd85d-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="dd85d-106">Trong **trang web đối tượng**, chọn **luồng**công việc.</span><span class="sxs-lookup"><span data-stu-id="dd85d-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="dd85d-107">Trong phần **mới** của ruy băng **quy** trình, chọn công **việc tái**sử dụng.</span><span class="sxs-lookup"><span data-stu-id="dd85d-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="dd85d-108">Trên biểu mẫu **tạo luồng công việc tái** sử dụng, hãy nhập tên \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="dd85d-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="dd85d-109">Đối với **loại nền tảng**, bấm **SharePoint 2010 luồng công việc**, và sau đó bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="dd85d-110">Trong phần **lưu** của ruy băng **luồng công việc** , chọn **xuất bản**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="dd85d-111">Trong phần **quản lý** của Ribbon **luồng công việc** , chọn **xuất bản toàn cầu**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="dd85d-112">Trong hộp thoại xác nhận xuất hiện, chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="dd85d-113">Trong một trình duyệt web, xác định vị trí trang web gốc của bộ sưu tập trang web, và sau đó truy cập trang web **thiết lập** \> **bộ sưu tập các tính năng**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="dd85d-114">Bật/tắt tính năng **luồng** công việc:</span><span class="sxs-lookup"><span data-stu-id="dd85d-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="dd85d-115">· Nếu tính năng được *kích hoạt* , bấm vô hiệu hóa **,** và sau đó bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="dd85d-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="dd85d-116">· Nếu tính năng bị *hủy* **kích hoạt**, hãy nhấp vào bật.</span><span class="sxs-lookup"><span data-stu-id="dd85d-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="dd85d-117">Để biết thêm thông tin, vui lòng tham khảo [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)sau đây.</span><span class="sxs-lookup"><span data-stu-id="dd85d-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

