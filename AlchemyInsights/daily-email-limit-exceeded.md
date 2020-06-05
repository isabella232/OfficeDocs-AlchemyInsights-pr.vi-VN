---
title: Vượt quá giới hạn email hàng ngày. Quy trình làm việc bị treo.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580355"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="31c91-103">Vượt quá giới hạn email hàng ngày.</span><span class="sxs-lookup"><span data-stu-id="31c91-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="31c91-104">Quy trình làm việc bị treo.</span><span class="sxs-lookup"><span data-stu-id="31c91-104">Workflow is suspended.</span></span>

<span data-ttu-id="31c91-105">Lỗi này có thể nhận được trong các trường hợp sau:</span><span class="sxs-lookup"><span data-stu-id="31c91-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="31c91-106">Bạn có một công việc trong SharePoint trực tuyến sử dụng loại nền tảng công việc SharePoint 2010 hoặc SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="31c91-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="31c91-107">Luồng công việc được cấu hình để gửi thư email tùy chỉnh cho hơn 200 người dùng tại một thời gian, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.</span><span class="sxs-lookup"><span data-stu-id="31c91-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="31c91-108">Khi bạn chạy luồng công việc, thư email không được gửi và bạn thấy hiện tượng sau:</span><span class="sxs-lookup"><span data-stu-id="31c91-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="31c91-109">Luồng công việc sử dụng loại nền tảng SharePoint 2013, bạn duyệt trang **trạng thái luồng công việc** .</span><span class="sxs-lookup"><span data-stu-id="31c91-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="31c91-110">Trên trang trạng thái luồng công việc, **trạng thái nội bộ** được thiết lập để **bắt đầu**, và bóng thông tin hiển thị **không thể gửi đến người nhận**.</span><span class="sxs-lookup"><span data-stu-id="31c91-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="31c91-111">Để khắc phục sự cố này, cấu hình luồng công việc của bạn để gửi thư điện tử mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="31c91-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="31c91-112">Ví dụ: sử dụng tạm dừng trong quy trình làm việc, gửi email tới nhóm Microsoft 365, nhóm phân phối hoặc nhóm bảo mật được kích hoạt thư hoặc gửi thư đến ít hơn 200 người nhận cùng một lúc.</span><span class="sxs-lookup"><span data-stu-id="31c91-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="31c91-113">Để biết thêm thông tin, hãy xem [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)sau.</span><span class="sxs-lookup"><span data-stu-id="31c91-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="31c91-114">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="31c91-114">Related topics</span></span>
- [<span data-ttu-id="31c91-115">Tạo Flow</span><span class="sxs-lookup"><span data-stu-id="31c91-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="31c91-116">SharePoint và Flow</span><span class="sxs-lookup"><span data-stu-id="31c91-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 