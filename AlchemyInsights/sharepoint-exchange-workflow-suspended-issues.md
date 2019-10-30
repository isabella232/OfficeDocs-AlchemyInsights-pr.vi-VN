---
title: Bắt đầu với SharePoint Online
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766913"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="0e623-102">Luồng công việc trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e623-102">Workflows in SharePoint</span></span>

<span data-ttu-id="0e623-103">Nếu luồng công việc SharePoint không gửi email, tổ chức của bạn có thể gặp phải giới hạn người gửi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0e623-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="0e623-104">Thông báo lỗi ' quy trình làm việc bị treo ' có thể xảy ra nếu bạn có một trong các mục sau:</span><span class="sxs-lookup"><span data-stu-id="0e623-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="0e623-105">Bạn có một công việc trong SharePoint trực tuyến sử dụng loại nền tảng công việc SharePoint 2010 hoặc SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="0e623-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="0e623-106">Luồng công việc được cấu hình để gửi thư email tùy chỉnh cho hơn 200 người dùng tại một thời gian, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.</span><span class="sxs-lookup"><span data-stu-id="0e623-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="0e623-107">Khi bạn chạy luồng công việc, thư email không được gửi và bạn thấy thông báo lỗi, trạng thái nội bộ nằm treo hoặc không thể gửi đến người nhận được hiển thị.</span><span class="sxs-lookup"><span data-stu-id="0e623-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="0e623-108">Để biết thêm thông tin, vui lòng tham khảo [bài viết](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)sau đây.</span><span class="sxs-lookup"><span data-stu-id="0e623-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

