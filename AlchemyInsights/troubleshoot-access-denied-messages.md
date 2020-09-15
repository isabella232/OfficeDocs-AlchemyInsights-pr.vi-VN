---
title: Khắc phục sự cố truy nhập thư bị từ chối
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690805"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="99d47-102">Khắc phục sự cố truy nhập thư bị từ chối</span><span class="sxs-lookup"><span data-stu-id="99d47-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="99d47-103">Nếu một người nào đó có thông báo "Access bị từ chối" vào một thư mục dùng chung trong SharePoint, người quản trị tuyển tập trang có thể đã bật chế độ người dùng có quyền truy nhập hạn chế ".</span><span class="sxs-lookup"><span data-stu-id="99d47-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="99d47-104">Để tắt tính năng này:</span><span class="sxs-lookup"><span data-stu-id="99d47-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="99d47-105">Duyệt đến site, bấm vào biểu tượng thiết đặt, rồi bấm **thiết đặt trang**.</span><span class="sxs-lookup"><span data-stu-id="99d47-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="99d47-106">Bên dưới **quản trị tuyển tập trang**, hãy bấm **tính năng tuyển tập trang**.</span><span class="sxs-lookup"><span data-stu-id="99d47-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="99d47-107">Bên cạnh **chế độ khóa quyền của người dùng truy nhập bị hạn chế**, hãy bấm **hủy**kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="99d47-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="99d47-108">Một thông báo bị từ chối truy nhập cũng có thể xảy ra đối với các thư mục dùng chung nếu site đó là một site phát hành.</span><span class="sxs-lookup"><span data-stu-id="99d47-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="99d47-109">Để biết thông tin, hãy xem [truy nhập bị từ chối khi truy nhập vào một thư mục dùng chung](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="99d47-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="99d47-110">Nếu một người nào đó có thông báo "truy nhập bị từ chối" khi tìm cách xem các yêu cầu truy nhập, thì người dùng cần phải được thêm vào như là người quản trị tuyển tập trang hoặc là thành viên của nhóm người sở hữu đối với site.</span><span class="sxs-lookup"><span data-stu-id="99d47-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="99d47-111">Để biết thêm thông tin, hãy xem [truy nhập bị từ chối vào danh sách yêu cầu truy nhập](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="99d47-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="99d47-112">Nếu người dùng có thông báo "truy nhập bị từ chối" sau khi chúng được loại bỏ khỏi Active Directory tại cơ sở và sau đó thêm lại, hãy xem [truy nhập bị từ chối khi tài khoản người dùng được đồng bộ hóa với Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="99d47-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

