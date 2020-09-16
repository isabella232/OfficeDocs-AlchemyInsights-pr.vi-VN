---
title: Vượt quá giới hạn email hàng ngày. Dòng công việc bị tạm ngừng.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731585"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="a6593-103">Vượt quá giới hạn email hàng ngày.</span><span class="sxs-lookup"><span data-stu-id="a6593-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="a6593-104">Dòng công việc bị tạm ngừng.</span><span class="sxs-lookup"><span data-stu-id="a6593-104">Workflow is suspended.</span></span>

<span data-ttu-id="a6593-105">Lỗi này có thể nhận được trong những tình huống sau đây:</span><span class="sxs-lookup"><span data-stu-id="a6593-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="a6593-106">Bạn có dòng công việc trong SharePoint Online vốn đang dùng kiểu nền tảng SharePoint 2010 hoặc SharePoint 2013 dòng công việc.</span><span class="sxs-lookup"><span data-stu-id="a6593-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="a6593-107">Dòng công việc được cấu hình để gửi thông điệp email tùy chỉnh cho hơn 200 người dùng cùng lúc, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.</span><span class="sxs-lookup"><span data-stu-id="a6593-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="a6593-108">Khi bạn chạy dòng công việc, thông điệp email không được gửi đi và bạn nhận thấy hành vi sau đây:</span><span class="sxs-lookup"><span data-stu-id="a6593-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="a6593-109">Đối với dòng công việc bằng cách dùng loại nền tảng SharePoint 2013, bạn duyệt đến trang **trạng thái** dòng công việc.</span><span class="sxs-lookup"><span data-stu-id="a6593-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="a6593-110">Trên trang trạng thái dòng công việc, **trạng thái nội bộ** được đặt thành **bắt đầu**và bóng chú thích sẽ hiển thị **không thể gửi cho người nhận**.</span><span class="sxs-lookup"><span data-stu-id="a6593-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="a6593-111">Để giải quyết vấn đề này, hãy cấu hình dòng công việc của bạn để gửi thư email mà không vượt quá [giới hạn người gửi Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="a6593-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="a6593-112">Ví dụ: sử dụng tạm dừng trong dòng công việc, gửi email đến một nhóm Microsoft 365, nhóm phân phối hoặc nhóm bảo mật cho phép thư hoặc gửi thư đến ít hơn 200 người nhận mỗi lần.</span><span class="sxs-lookup"><span data-stu-id="a6593-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="a6593-113">Để biết thêm thông tin, hãy xem [bài viết](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)sau đây.</span><span class="sxs-lookup"><span data-stu-id="a6593-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="a6593-114">Chủ đề liên quan</span><span class="sxs-lookup"><span data-stu-id="a6593-114">Related topics</span></span>
- [<span data-ttu-id="a6593-115">Tạo dòng</span><span class="sxs-lookup"><span data-stu-id="a6593-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a6593-116">SharePoint và dòng</span><span class="sxs-lookup"><span data-stu-id="a6593-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 