---
title: Truy nhập bị từ chối khi xem luồng công việc
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747770"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="a157d-102">Truy nhập bị từ chối khi xem luồng công việc</span><span class="sxs-lookup"><span data-stu-id="a157d-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="a157d-103">SharePoint 2013 luồng công việc cố gắng gửi email đến một nhóm SharePoint có thể thất bại với thông báo lỗi "truy cập từ chối" nếu các thành viên của nhóm SharePoint không được đặt thành tất cả mọi người.</span><span class="sxs-lookup"><span data-stu-id="a157d-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="a157d-104">**Để khắc phục sự cố này, thực hiện các bước sau:**</span><span class="sxs-lookup"><span data-stu-id="a157d-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="a157d-105">Cho phép tất cả mọi người xem các thành viên của nhóm SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a157d-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="a157d-106">Loại bỏ nhóm SharePoint từ hoặc CC dòng email.</span><span class="sxs-lookup"><span data-stu-id="a157d-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="a157d-107">Rõ ràng thêm người dùng đến hoặc CC dòng nếu Hiển thị thành viên không thể thay đổi cho nhóm SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a157d-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="a157d-108">Để xem thêm chi tiết xin vui lòng tham khảo [http trái phép để/_vti_bin/client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="a157d-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  