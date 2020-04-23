---
title: Đồng bộ hóa hồ sơ
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768135"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a6cbf-102">Khi nào hồ sơ của tôi thay đổi đồng bộ hóa với ứng dụng hồ sơ người dùng SharePoint?</span><span class="sxs-lookup"><span data-stu-id="a6cbf-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a6cbf-103">SharePoint Online sử dụng công việc giờ Active Directory nhập (AD nhập) để nhập người dùng và nhóm vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a6cbf-104">AD nhập đồng bộ thay đổi từ cửa hàng trực tuyến SharePoint vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="a6cbf-105">Những thay đổi này được xử lý theo lô.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a6cbf-106">Việc hẹn giờ chạy cho đến khi các thay đổi được đồng bộ hóa.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a6cbf-107">Thời gian phải mất công việc để chạy phụ thuộc vào số lượng thay đổi để xử lý.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="a6cbf-108">Một số lượng lớn các thay đổi mất nhiều thời gian hơn.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-108">A large number of changes takes longer.</span></span> <span data-ttu-id="a6cbf-109">Thỏa thuận mức dịch vụ (SLA) cho biết thay đổi cho người dùng trong thư mục SharePoint trực tuyến sẽ được phản ánh trong ứng dụng hồ sơ người dùng trong 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="a6cbf-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a6cbf-110">Thông tin thêm về đồng bộ hóa hồ sơ người dùng trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="a6cbf-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

