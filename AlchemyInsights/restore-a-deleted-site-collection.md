---
title: Khôi phục site đã xóa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692065"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="f4a32-102">Khôi phục site đã xóa</span><span class="sxs-lookup"><span data-stu-id="f4a32-102">Restore a deleted site</span></span>

<span data-ttu-id="f4a32-103">Khi người quản trị xóa bỏ một site SharePoint, nó sẽ được đặt trong thùng rác của tuyển tập site, nơi nó được lưu trữ trong 93 ngày trước khi nó bị xóa vĩnh viễn.</span><span class="sxs-lookup"><span data-stu-id="f4a32-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="f4a32-104">Để khôi phục site:</span><span class="sxs-lookup"><span data-stu-id="f4a32-104">To restore the site:</span></span>
  
1. <span data-ttu-id="f4a32-105">Trong Trung tâm quản trị SharePoint mới, hãy bấm **thùng rác** trên dải băng.</span><span class="sxs-lookup"><span data-stu-id="f4a32-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="f4a32-106">Chọn hộp kiểm bên cạnh tuyển tập trang bạn muốn khôi phục.</span><span class="sxs-lookup"><span data-stu-id="f4a32-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="f4a32-107">Bấm **khôi phục các mục đã xóa**.</span><span class="sxs-lookup"><span data-stu-id="f4a32-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="f4a32-108">Để khôi phục một site liên lạc đã xóa, bạn có thể sử dụng trung tâm quản trị SharePoint mới.</span><span class="sxs-lookup"><span data-stu-id="f4a32-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="f4a32-109">Nếu không, bạn cần sử dụng Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f4a32-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="f4a32-110">Để khôi phục một site thuộc nhóm Microsoft 365, bạn cần khôi phục nhóm trong Trung tâm quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4a32-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="f4a32-111">Các nhóm có thể được khôi phục trong 30 ngày sau khi xóa.</span><span class="sxs-lookup"><span data-stu-id="f4a32-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

