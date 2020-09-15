---
title: Đồng bộ hóa hồ sơ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801791"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="fe941-102">Khi nào hồ sơ của tôi thay đổi đồng bộ với ứng dụng hồ sơ người dùng SharePoint?</span><span class="sxs-lookup"><span data-stu-id="fe941-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="fe941-103">SharePoint Online sử dụng công việc hẹn giờ nhập Active Directory (nhập vào quảng cáo) để nhập người dùng và nhóm vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="fe941-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="fe941-104">Người đồng bộ nhập quảng cáo thay đổi từ kho lưu trữ thư mục SharePoint Online vào ứng dụng hồ sơ người dùng.</span><span class="sxs-lookup"><span data-stu-id="fe941-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="fe941-105">Những thay đổi này được xử lý theo lô.</span><span class="sxs-lookup"><span data-stu-id="fe941-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="fe941-106">Công việc hẹn giờ sẽ chạy cho đến khi các thay đổi được đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="fe941-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="fe941-107">Thời gian cần thiết để chạy công việc phụ thuộc vào số lượng thay đổi thành quy trình.</span><span class="sxs-lookup"><span data-stu-id="fe941-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="fe941-108">Một số lượng lớn các thay đổi sẽ kéo dài lâu hơn.</span><span class="sxs-lookup"><span data-stu-id="fe941-108">A large number of changes takes longer.</span></span> <span data-ttu-id="fe941-109">Thỏa thuận mức dịch vụ (SLA) nói rằng một thay đổi đối với người dùng trong thư mục SharePoint Online sẽ được phản ánh trong ứng dụng hồ sơ người dùng trong 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="fe941-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="fe941-110">Thông tin thêm về đồng bộ hóa hồ sơ người dùng trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="fe941-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

