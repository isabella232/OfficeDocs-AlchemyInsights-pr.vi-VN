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
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558014"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="a2816-102">Công việc không bắt đầu</span><span class="sxs-lookup"><span data-stu-id="a2816-102">Workflow is not starting</span></span>

- <span data-ttu-id="a2816-103">SharePoint 2010 và SharePoint 2013 quy trình công việc không bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="a2816-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="a2816-104">Nếu công việc của bạn không bắt đầu, có thể có một vấn đề tạm thời dịch vụ nơi người dùng có thể trải nghiệm sự chậm trễ liên tục với tiến độ công việc.</span><span class="sxs-lookup"><span data-stu-id="a2816-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="a2816-105">Kiểm tra [Bảng điều khiển dịch vụ y tế](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem nếu tổ chức của bạn bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="a2816-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="a2816-106">Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="a2816-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="a2816-107">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="a2816-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="a2816-108">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="a2816-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="a2816-109">SharePoint 2010 quy trình công việc trì hoãn ngày bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="a2816-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="a2816-110">Điều này xảy ra nếu các công việc được kích hoạt trong lô lớn.</span><span class="sxs-lookup"><span data-stu-id="a2816-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="a2816-111">(ví dụ, khi một số khoản mục được thêm vào cùng một lúc).</span><span class="sxs-lookup"><span data-stu-id="a2816-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="a2816-112">Quy trình công việc không được thiết kế để chạy thời gian thực, do đó, một sự chậm trễ là hành vi của thiết kế.</span><span class="sxs-lookup"><span data-stu-id="a2816-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="a2816-113">Nếu công việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), trình biên dịch có thể được làm chậm.</span><span class="sxs-lookup"><span data-stu-id="a2816-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="a2816-114">Kiểm tra bài viết [này](https://support.microsoft.com/en-us/kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="a2816-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    - <span data-ttu-id="a2816-115">Bạn nên đơn giản hóa các công việc hoặc thiết kế lại nó bằng cách sử dụng các loại nền tảng Microsoft SharePoint 2013 quy trình làm việc.</span><span class="sxs-lookup"><span data-stu-id="a2816-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="a2816-116">Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các khoản mục hoặc tạo ra một danh sách lịch sử mới.</span><span class="sxs-lookup"><span data-stu-id="a2816-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="a2816-117">Thông tin thêm: [dọn sạch các lịch sử công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="a2816-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="a2816-118">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="a2816-118">Related topics</span></span>
<span data-ttu-id="a2816-119">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="a2816-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a2816-120">Tạo ra dòng chảy</span><span class="sxs-lookup"><span data-stu-id="a2816-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a2816-121">SharePoint và dòng chảy</span><span class="sxs-lookup"><span data-stu-id="a2816-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


