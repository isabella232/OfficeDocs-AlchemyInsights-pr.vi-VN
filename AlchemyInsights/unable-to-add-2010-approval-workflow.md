---
title: Không thể thêm năm 2010 phê duyệt quy trình làm việc
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28321293"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="6f1fb-102">Không thể thêm năm 2010 phê duyệt quy trình làm việc</span><span class="sxs-lookup"><span data-stu-id="6f1fb-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="6f1fb-103">Trong một bộ sưu tập trang web Microsoft SharePoint, bạn không thể thêm một công việc toàn cầu tái sử dụng (ví dụ như "phê duyệt - SharePoint 2010") một danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="6f1fb-104">Để giải quyết vấn đề này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="6f1fb-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="6f1fb-105">Mở trang web gốc của bộ sưu tập trang web trong SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="6f1fb-106">Theo **Các đối tượng trang web**, hãy chọn **công việc**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="6f1fb-107">Trong phần **mới** của ribbon **quy trình công việc** , hãy chọn **Công việc tái sử dụng**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="6f1fb-p101">Các hình thức **Tạo ra công việc tái sử dụng** , hãy nhập tên \*\* *Repair2010* \*\*. Đối với **Nền tảng loại**, nhấp vào **Quy trình làm việc SharePoint 2010**, và sau đó bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="6f1fb-110">Trong phần **lưu** của ribbon **luồng công việc** , chọn **xuất bản**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="6f1fb-p102">Trong phần **quản lý** các ribbon **luồng công việc** , chọn **Xuất bản trên toàn cầu**. Trong hộp thoại xác nhận xuất hiện, chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="6f1fb-p103">Trình duyệt web, xác định vị trí các trang web gốc của bộ sưu tập trang web, và sau đó truy cập vào **Thiết lập trang web** \> **Tính năng bộ sưu tập trang web**. Bật/tắt tính năng **công việc** :</span><span class="sxs-lookup"><span data-stu-id="6f1fb-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="6f1fb-115">· Nếu các tính năng là *kích hoạt* , hãy nhấp vào **vô hiệu hóa,** và sau đó nhấp vào **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="6f1fb-116">· Nếu các tính năng *Deactivated* , bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="6f1fb-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="6f1fb-117">Thông tin chi tiết vui lòng tham khảo sau đây [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="6f1fb-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

