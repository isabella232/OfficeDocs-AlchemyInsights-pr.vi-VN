---
title: Bắt đầu với SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700729"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="13b53-102">Dòng công việc trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="13b53-102">Workflows in SharePoint</span></span>

<span data-ttu-id="13b53-103">Nếu dòng công việc SharePoint không gửi email, tổ chức của bạn có thể đã gặp phải giới hạn người gửi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="13b53-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="13b53-104">Thông báo lỗi ' dòng công việc bị tạm ngừng có thể xảy ra nếu bạn có một trong các mục sau đây:</span><span class="sxs-lookup"><span data-stu-id="13b53-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="13b53-105">Bạn có dòng công việc trong SharePoint Online vốn đang dùng kiểu nền tảng SharePoint 2010 hoặc SharePoint 2013 dòng công việc.</span><span class="sxs-lookup"><span data-stu-id="13b53-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="13b53-106">Dòng công việc được cấu hình để gửi thông điệp email tùy chỉnh cho hơn 200 người dùng cùng lúc, hơn 10.000 người nhận mỗi ngày, hoặc hơn 30 thư mỗi phút.</span><span class="sxs-lookup"><span data-stu-id="13b53-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="13b53-107">Khi bạn chạy dòng công việc, thông điệp email không được gửi đi và bạn nhận thấy thông báo lỗi, trạng thái nội bộ được đặt là bị tạm ngừng hoặc không thể gửi đến người nhận được hiển thị.</span><span class="sxs-lookup"><span data-stu-id="13b53-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="13b53-108">Để biết thêm thông tin, vui lòng tham khảo [bài viết](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)sau đây.</span><span class="sxs-lookup"><span data-stu-id="13b53-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

