---
title: Luồng công việc không bắt đầu
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
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738111"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="b83d6-102">Luồng công việc không bắt đầu</span><span class="sxs-lookup"><span data-stu-id="b83d6-102">Workflow is not starting</span></span>

- <span data-ttu-id="b83d6-103">SharePoint 2010 và SharePoint 2013 luồng công việc không khởi chạy.</span><span class="sxs-lookup"><span data-stu-id="b83d6-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="b83d6-104">Nếu công việc của bạn không khởi động, có thể có sự cố dịch vụ tạm thời mà người dùng có thể gặp phải gián đoạn liên tục với tiến trình luồng công việc.</span><span class="sxs-lookup"><span data-stu-id="b83d6-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="b83d6-105">Kiểm tra [bảng điều khiển tình trạng dịch vụ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.</span><span class="sxs-lookup"><span data-stu-id="b83d6-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="b83d6-106">Nếu hơn 24 giờ đã trôi qua kể từ lần đầu tiên bạn thấy vấn đề này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="b83d6-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="b83d6-107">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="b83d6-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b83d6-108">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="b83d6-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="b83d6-109">Luồng công việc SharePoint 2010 chậm trễ trên bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="b83d6-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="b83d6-110">Điều này xảy ra nếu công việc được kích hoạt trong lô lớn.</span><span class="sxs-lookup"><span data-stu-id="b83d6-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="b83d6-111">(ví dụ: khi một số mục được thêm vào cùng một lúc).</span><span class="sxs-lookup"><span data-stu-id="b83d6-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="b83d6-112">Luồng công việc không được thiết kế để chạy thời gian thực, do đó, sự chậm trễ là hành vi thiết kế.</span><span class="sxs-lookup"><span data-stu-id="b83d6-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="b83d6-113">Nếu quy trình làm việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), biên soạn có thể chậm.</span><span class="sxs-lookup"><span data-stu-id="b83d6-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="b83d6-114">Kiểm tra bài viết [này](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="b83d6-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="b83d6-115">Bạn nên đơn giản hóa công việc hoặc thiết kế lại nó bằng cách sử dụng loại nền tảng Microsoft SharePoint 2013 luồng công việc.</span><span class="sxs-lookup"><span data-stu-id="b83d6-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="b83d6-116">Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các mục hoặc tạo danh sách lịch sử mới.</span><span class="sxs-lookup"><span data-stu-id="b83d6-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="b83d6-117">Thông tin thêm: [xoá lịch sử luồng công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="b83d6-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="b83d6-118">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="b83d6-118">Related topics</span></span>
<span data-ttu-id="b83d6-119">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="b83d6-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="b83d6-120">Tạo Flow</span><span class="sxs-lookup"><span data-stu-id="b83d6-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="b83d6-121">SharePoint và Flow</span><span class="sxs-lookup"><span data-stu-id="b83d6-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


