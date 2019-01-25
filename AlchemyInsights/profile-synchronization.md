---
title: Đồng bộ hóa Profile
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29497394"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="14aa0-102">Khi làm thay đổi cấu hình của mình đồng bộ ứng dụng hồ sơ người dùng SharePoint?</span><span class="sxs-lookup"><span data-stu-id="14aa0-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="14aa0-103">SharePoint Online sử dụng hoạt động thư mục nhập khẩu bộ đếm thời gian công việc (AD nhập khẩu) để nhập người dùng và nhóm vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="14aa0-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="14aa0-p101">Quảng cáo nhập khẩu đồng bộ các thay đổi từ các cửa hàng thư mục trực tuyến SharePoint để ứng dụng hồ sơ người dùng. Những thay đổi này được xử lý theo lô.</span><span class="sxs-lookup"><span data-stu-id="14aa0-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="14aa0-106">Việc đếm thời gian chạy cho đến khi các thay đổi được đồng bộ hóa.</span><span class="sxs-lookup"><span data-stu-id="14aa0-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="14aa0-p102">Thời gian công việc để chạy phụ thuộc vào số lượng thay đổi để xử lý. Một số lượng lớn các thay đổi mất nhiều thời gian. Thỏa thuận cấp độ dịch vụ (SLA) nói rằng một sự thay đổi cho người dùng trong thư mục trực tuyến SharePoint sẽ được phản ánh trong ứng dụng hồ sơ người dùng trong 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="14aa0-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="14aa0-110">Thông tin thêm về đồng bộ hồ sơ người dùng SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="14aa0-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

