---
title: Truy cập từ chối khi xem một công việc
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 43369c600687d6ac253f70a8535dc2bd0d41687e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918850"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="b5781-102">Truy cập từ chối khi xem một công việc</span><span class="sxs-lookup"><span data-stu-id="b5781-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="b5781-103">SharePoint 2013 quy trình công việc mà cố gắng để gửi email đến một nhóm SharePoint có thể thất bại với một thông báo lỗi "Truy cập từ chối" nếu các thành viên của nhóm SharePoint không được thiết lập để tất cả mọi người.</span><span class="sxs-lookup"><span data-stu-id="b5781-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="b5781-104">**Để giải quyết vấn đề này, hãy làm các bước sau:**</span><span class="sxs-lookup"><span data-stu-id="b5781-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="b5781-105">Cho phép tất cả mọi người để xem các thành viên của nhóm SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b5781-105">Allow everybody to see the members of the SharePoint group.</span></span> 
  
 2. <span data-ttu-id="b5781-106">Loại bỏ nhóm SharePoint từ k/g hoặc sao của email.</span><span class="sxs-lookup"><span data-stu-id="b5781-106">Remove the SharePoint group from the To or CC line of the email.</span></span> 
  
 3. <span data-ttu-id="b5781-107">Một cách rõ ràng thêm người dùng k/g hoặc sao dòng nếu tầm nhìn của thành viên không thể thay đổi cho SharePoint group.</span><span class="sxs-lookup"><span data-stu-id="b5781-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span> 
  
<span data-ttu-id="b5781-108">Để xem thêm chi tiết xin vui lòng tham khảo [HTTP trái phép để /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="b5781-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  

