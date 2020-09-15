---
title: Truy nhập bị từ chối khi xem dòng công việc
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688824"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="6a196-102">Truy nhập bị từ chối khi xem dòng công việc</span><span class="sxs-lookup"><span data-stu-id="6a196-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="6a196-103">Dòng công việc SharePoint 2013 cố gắng gửi email đến một nhóm SharePoint có thể không thành công với thông báo lỗi "truy nhập bị từ chối" nếu là thành viên của nhóm SharePoint không được đặt là tất cả mọi người.</span><span class="sxs-lookup"><span data-stu-id="6a196-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="6a196-104">**Để giải quyết vấn đề này, hãy thực hiện các bước sau:**</span><span class="sxs-lookup"><span data-stu-id="6a196-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="6a196-105">Cho phép mọi người nhìn thấy các thành viên của nhóm SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6a196-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="6a196-106">Loại bỏ nhóm SharePoint khỏi dòng đến hoặc CC của email.</span><span class="sxs-lookup"><span data-stu-id="6a196-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="6a196-107">Rõ ràng thêm người dùng vào dòng đến hoặc CC nếu không thể thay đổi khả năng hiển thị thành viên cho nhóm SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6a196-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="6a196-108">Để xem thêm chi tiết, vui lòng tham khảo http không được [phép đến/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="6a196-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  