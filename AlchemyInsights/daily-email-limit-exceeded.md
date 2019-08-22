---
title: Giới hạn email hàng ngày vượt quá. Công việc bị đình chỉ.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514497"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="34614-103">Hàng ngày email vượt quá giới hạn.</span><span class="sxs-lookup"><span data-stu-id="34614-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="34614-104">Công việc bị đình chỉ.</span><span class="sxs-lookup"><span data-stu-id="34614-104">Workflow is suspended.</span></span>

<span data-ttu-id="34614-105">Lỗi này có thể nhận được trong các trường hợp sau:</span><span class="sxs-lookup"><span data-stu-id="34614-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="34614-106">Bạn có một công việc trong SharePoint Online, sử dụng SharePoint 2010 hoặc SharePoint 2013 công việc nền tảng loại.</span><span class="sxs-lookup"><span data-stu-id="34614-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="34614-107">Các công việc được cấu hình để gửi một tin nhắn tuỳ chỉnh email cho hơn 200 người dùng tại một thời gian, hơn 10.000 người nhận mỗi ngày hoặc nhiều hơn 30 thư mỗi phút.</span><span class="sxs-lookup"><span data-stu-id="34614-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="34614-108">Khi bạn chạy quy trình làm việc, thông báo email không được gửi và bạn thông báo các hành vi sau đây:</span><span class="sxs-lookup"><span data-stu-id="34614-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="34614-109">Cho một công việc bằng cách sử dụng các loại nền tảng SharePoint 2013, bạn duyệt đến trang **Tình trạng luồng công việc** .</span><span class="sxs-lookup"><span data-stu-id="34614-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="34614-110">Trên trang tình trạng công việc, **Tình trạng nội bộ** được thiết lập để **bắt đầu**, và hiển thị thông tin bóng **không thể gửi đến người nhận**.</span><span class="sxs-lookup"><span data-stu-id="34614-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="34614-111">Để làm việc xung quanh vấn đề này, đặt cấu hình công việc của bạn để gửi thư điện tử mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="34614-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="34614-112">Ví dụ, sử dụng một tạm dừng trong công việc, gửi email cho một nhóm Office 365, một nhóm phân phối hoặc nhóm bảo mật được kích hoạt thư hoặc gửi tin nhắn đến ít hơn 200 người nhận tại một thời điểm.</span><span class="sxs-lookup"><span data-stu-id="34614-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="34614-113">Để biết thêm chi tiết, xem sau đây [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="34614-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="34614-114">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="34614-114">Related topics</span></span>
- [<span data-ttu-id="34614-115">Tạo ra dòng chảy</span><span class="sxs-lookup"><span data-stu-id="34614-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="34614-116">SharePoint và dòng chảy</span><span class="sxs-lookup"><span data-stu-id="34614-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 