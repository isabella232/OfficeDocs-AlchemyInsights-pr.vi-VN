---
title: Luồng công việc không bắt đầu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766119"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="cf2e9-102">Luồng công việc không bắt đầu</span><span class="sxs-lookup"><span data-stu-id="cf2e9-102">Workflow is not starting</span></span>

- <span data-ttu-id="cf2e9-103">SharePoint 2010 và SharePoint 2013 luồng công việc không khởi chạy.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="cf2e9-104">Nếu công việc của bạn không khởi động, có thể có sự cố dịch vụ tạm thời mà người dùng có thể gặp phải gián đoạn liên tục với tiến trình luồng công việc.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="cf2e9-105">Kiểm tra [bảng điều khiển tình trạng dịch vụ](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="cf2e9-106">Nếu hơn 24 giờ đã trôi qua kể từ lần đầu tiên bạn thấy vấn đề này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="cf2e9-107">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="cf2e9-108">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="cf2e9-109">Luồng công việc SharePoint 2010 chậm trễ trên bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="cf2e9-110">Điều này xảy ra nếu công việc được kích hoạt trong lô lớn.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="cf2e9-111">(ví dụ: khi một số mục được thêm vào cùng một lúc).</span><span class="sxs-lookup"><span data-stu-id="cf2e9-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="cf2e9-112">Luồng công việc không được thiết kế để chạy thời gian thực, do đó, sự chậm trễ là hành vi thiết kế.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="cf2e9-113">Nếu quy trình làm việc phức tạp mở rộng đối tượng đánh dấu ngôn ngữ (XMOL), biên soạn có thể chậm.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="cf2e9-114">Kiểm tra bài viết [này](https://support.microsoft.com//kb/3043697) .</span><span class="sxs-lookup"><span data-stu-id="cf2e9-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="cf2e9-115">Bạn nên đơn giản hóa công việc hoặc thiết kế lại nó bằng cách sử dụng loại nền tảng Microsoft SharePoint 2013 luồng công việc.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="cf2e9-116">Nếu lịch sử công việc của bạn đã phát triển lớn, bạn có thể muốn xoá các mục hoặc tạo danh sách lịch sử mới.</span><span class="sxs-lookup"><span data-stu-id="cf2e9-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="cf2e9-117">Thông tin thêm: [xoá lịch sử luồng công việc](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="cf2e9-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="cf2e9-118">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="cf2e9-118">Related topics</span></span>
<span data-ttu-id="cf2e9-119">Bạn muốn thử Microsoft Flow trong SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="cf2e9-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="cf2e9-120">Tạo Flow</span><span class="sxs-lookup"><span data-stu-id="cf2e9-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="cf2e9-121">SharePoint và Flow</span><span class="sxs-lookup"><span data-stu-id="cf2e9-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


