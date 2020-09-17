---
title: Không bắt đầu dòng công việc
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794789"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="8e024-102">Không bắt đầu dòng công việc</span><span class="sxs-lookup"><span data-stu-id="8e024-102">Workflow is not starting</span></span>

- <span data-ttu-id="8e024-103">Dòng công việc SharePoint 2010 và dòng công việc SharePoint 2013 không bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="8e024-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="8e024-104">Nếu dòng công việc của bạn không bắt đầu, có thể có sự cố dịch vụ tạm thời mà người dùng có thể gặp phải sự chậm trễ với dòng công việc.</span><span class="sxs-lookup"><span data-stu-id="8e024-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="8e024-105">Kiểm tra [bảng điều khiển trạng thái dịch vụ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.</span><span class="sxs-lookup"><span data-stu-id="8e024-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="8e024-106">Nếu đã trôi qua 24 giờ kể từ lần đầu tiên bạn gặp sự cố này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="8e024-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8e024-107">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="8e024-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8e024-108">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="8e024-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="8e024-109">Dòng công việc SharePoint 2010 bị trì hoãn khi bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="8e024-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="8e024-110">Điều này xảy ra nếu dòng công việc được kích hoạt trong lô lớn.</span><span class="sxs-lookup"><span data-stu-id="8e024-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="8e024-111">(ví dụ, khi một số mục được thêm vào một lần).</span><span class="sxs-lookup"><span data-stu-id="8e024-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="8e024-112">Dòng công việc không được thiết kế để chạy theo thời gian thực, do đó, một hành vi chậm trễ là do thiết kế.</span><span class="sxs-lookup"><span data-stu-id="8e024-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="8e024-113">Nếu dòng công việc được mở rộng phức tạp là ngôn ngữ đánh dấu đối tượng (XMOL), thì bạn có thể làm chậm trình tổng hợp.</span><span class="sxs-lookup"><span data-stu-id="8e024-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="8e024-114">Kiểm tra bài viết [này](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="8e024-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="8e024-115">Bạn nên đơn giản hóa dòng công việc hoặc thiết kế lại bằng cách dùng loại nền tảng dòng công việc Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="8e024-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="8e024-116">Nếu lịch sử dòng công việc của bạn đã trưởng thành lớn, bạn có thể muốn tẩy các mục hoặc tạo danh sách lịch sử mới.</span><span class="sxs-lookup"><span data-stu-id="8e024-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="8e024-117">Thông tin thêm: [dọn sạch lịch sử](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/) dòng công việc</span><span class="sxs-lookup"><span data-stu-id="8e024-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="8e024-118">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="8e024-118">Related topics</span></span>
<span data-ttu-id="8e024-119">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="8e024-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="8e024-120">Tạo dòng</span><span class="sxs-lookup"><span data-stu-id="8e024-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="8e024-121">SharePoint và dòng</span><span class="sxs-lookup"><span data-stu-id="8e024-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


