---
title: Không thể thêm dòng công việc phê duyệt 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699757"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="34b09-102">Không thể thêm dòng công việc phê duyệt 2010</span><span class="sxs-lookup"><span data-stu-id="34b09-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="34b09-103">Trong tuyển tập trang Microsoft SharePoint, bạn không thể thêm dòng công việc thể dùng lại trên toàn cầu (chẳng hạn như "phê duyệt-SharePoint 2010") vào danh sách hoặc thư viện.</span><span class="sxs-lookup"><span data-stu-id="34b09-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="34b09-104">Để giải quyết vấn đề này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="34b09-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="34b09-105">Mở trang web gốc của tuyển tập site trong SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="34b09-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="34b09-106">Bên dưới **đối tượng site**, hãy chọn **dòng**công việc.</span><span class="sxs-lookup"><span data-stu-id="34b09-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="34b09-107">Trong phần **mới** của Ribbon **dòng** công việc, hãy chọn dòng công việc có thể **sử**dụng lại.</span><span class="sxs-lookup"><span data-stu-id="34b09-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="34b09-108">Trên biểu mẫu tạo dòng công việc có thể **tái sử** dụng, hãy nhập tên \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="34b09-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="34b09-109">Đối với **loại nền tảng**, bấm dòng công việc **SharePoint 2010**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="34b09-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="34b09-110">Trong phần **lưu** **của Ribbon dòng công việc** **, hãy chọn**phát hành.</span><span class="sxs-lookup"><span data-stu-id="34b09-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="34b09-111">Trong phần **quản lý** **của ruy-** băng dòng công việc, chọn phát hành **trên toàn cầu**.</span><span class="sxs-lookup"><span data-stu-id="34b09-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="34b09-112">Trong hộp thoại xác nhận xuất hiện, hãy chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="34b09-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="34b09-113">Trong trình duyệt web, hãy định vị trang web gốc của tuyển tập trang, rồi **Site Settings** truy nhập các \> **tính năng của tuyển tập**trang thiết đặt trang.</span><span class="sxs-lookup"><span data-stu-id="34b09-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="34b09-114">Bật/tắt tính năng **dòng** công việc:</span><span class="sxs-lookup"><span data-stu-id="34b09-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="34b09-115">· Nếu tính năng này được  *kích hoạt*  , hãy bấm Hủy kích hoạt **,** rồi bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="34b09-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="34b09-116">· Nếu tính năng này bị  *hủy kích hoạt*  , hãy bấm **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="34b09-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="34b09-117">Để biết thêm thông tin, vui lòng tham khảo [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)sau đây.</span><span class="sxs-lookup"><span data-stu-id="34b09-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

