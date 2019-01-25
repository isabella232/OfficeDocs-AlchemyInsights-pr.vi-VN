---
title: Không thể thêm mặc định năm 2010 phê duyệt quy trình làm việc
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496563"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="eea71-102">Không thể thêm mặc định năm 2010 phê duyệt quy trình làm việc</span><span class="sxs-lookup"><span data-stu-id="eea71-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="eea71-103">Trong một bộ sưu tập trang web Microsoft SharePoint, bạn không thể thêm một công việc toàn cầu tái sử dụng (ví dụ như "phê duyệt - SharePoint 2010") một danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="eea71-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="eea71-104">Để giải quyết vấn đề này, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="eea71-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="eea71-105">Mở trang web gốc của bộ sưu tập trang web trong SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="eea71-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="eea71-106">Theo **Các đối tượng trang web**, hãy chọn **công việc**.</span><span class="sxs-lookup"><span data-stu-id="eea71-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="eea71-107">Trong phần **mới** của ribbon **quy trình công việc** , hãy chọn **Công việc tái sử dụng**.</span><span class="sxs-lookup"><span data-stu-id="eea71-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="eea71-p101">Các hình thức **Tạo ra công việc tái sử dụng** , hãy nhập tên \* \*\*Repair2010\*\*\*. Đối với **Nền tảng loại**, chọn **SharePoint 2010 quy trình làm việc**, và sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="eea71-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="eea71-110">Trong phần **lưu** của ribbon **luồng công việc** , chọn **xuất bản**.</span><span class="sxs-lookup"><span data-stu-id="eea71-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="eea71-p102">Trong phần **quản lý** các ribbon **luồng công việc** , chọn **Xuất bản trên toàn cầu**. Trong hộp thoại xác nhận xuất hiện, chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="eea71-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="eea71-p103">Trình duyệt web, xác định vị trí các trang web gốc của bộ sưu tập trang web, và sau đó truy cập vào **Thiết lập trang web** \> **Tính năng bộ sưu tập trang web**. Sau đó, bật/tắt tính năng **công việc** :</span><span class="sxs-lookup"><span data-stu-id="eea71-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="eea71-115">· Nếu các tính năng là *kích hoạt* , hãy nhấp vào **vô hiệu hóa,** và sau đó nhấp vào **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="eea71-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="eea71-116">· Nếu các tính năng *Deactivated* , bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="eea71-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="eea71-117">Thông tin chi tiết vui lòng tham khảo sau đây [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="eea71-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

