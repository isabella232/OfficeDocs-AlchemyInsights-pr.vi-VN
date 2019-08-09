---
title: Công việc không bắt đầu
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270802"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="143a5-102">Công việc không bắt đầu</span><span class="sxs-lookup"><span data-stu-id="143a5-102">Workflow is not starting</span></span>

- <span data-ttu-id="143a5-103">SharePoint 2010 và SharePoint 2013 quy trình công việc không bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="143a5-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="143a5-104">Nếu công việc của bạn không bắt đầu, có thể có một vấn đề tạm thời dịch vụ nơi người dùng có thể trải nghiệm sự chậm trễ liên tục với tiến độ công việc.</span><span class="sxs-lookup"><span data-stu-id="143a5-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="143a5-105">Kiểm tra [Bảng điều khiển dịch vụ y tế](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem nếu tổ chức của bạn bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="143a5-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="143a5-106">Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="143a5-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="143a5-107">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="143a5-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="143a5-108">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="143a5-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="143a5-109">SharePoint 2010 quy trình công việc trì hoãn ngày bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="143a5-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="143a5-110">Điều này xảy ra nếu các công việc được kích hoạt trong lô lớn.</span><span class="sxs-lookup"><span data-stu-id="143a5-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="143a5-111">(ví dụ, khi một số khoản mục được thêm vào cùng một lúc).</span><span class="sxs-lookup"><span data-stu-id="143a5-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="143a5-112">Quy trình công việc không được thiết kế để chạy thời gian thực, do đó, một sự chậm trễ là hành vi của thiết kế.</span><span class="sxs-lookup"><span data-stu-id="143a5-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="143a5-113">Nếu công việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), trình biên dịch có thể được làm chậm.</span><span class="sxs-lookup"><span data-stu-id="143a5-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="143a5-114">Kiểm tra bài viết [này](https://support.microsoft.com/en-us/kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="143a5-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="143a5-115">Bạn nên đơn giản hóa các công việc hoặc thiết kế lại nó bằng cách sử dụng các loại nền tảng Microsoft SharePoint 2013 quy trình làm việc.</span><span class="sxs-lookup"><span data-stu-id="143a5-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="143a5-116">Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các khoản mục hoặc tạo ra một danh sách lịch sử mới.</span><span class="sxs-lookup"><span data-stu-id="143a5-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="143a5-117">Thông tin thêm: [dọn sạch các lịch sử công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="143a5-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="143a5-118">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="143a5-118">Related topics</span></span>
<span data-ttu-id="143a5-119">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="143a5-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="143a5-120">Tạo ra dòng chảy</span><span class="sxs-lookup"><span data-stu-id="143a5-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="143a5-121">SharePoint và dòng chảy</span><span class="sxs-lookup"><span data-stu-id="143a5-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


