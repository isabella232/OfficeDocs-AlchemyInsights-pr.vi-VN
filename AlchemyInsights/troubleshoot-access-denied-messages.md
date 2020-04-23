---
title: Khắc phục sự cố truy cập từ chối thư
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759822"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="e40bf-102">Khắc phục sự cố truy cập từ chối thư</span><span class="sxs-lookup"><span data-stu-id="e40bf-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="e40bf-103">Nếu ai đó nhận được thông báo "truy cập từ chối" vào một thư mục được chia sẻ trong SharePoint, quản trị viên bộ sưu tập trang web có thể đã kích hoạt "chế độ khoá quyền truy cập người dùng giới hạn."</span><span class="sxs-lookup"><span data-stu-id="e40bf-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="e40bf-104">Để tắt tính năng này:</span><span class="sxs-lookup"><span data-stu-id="e40bf-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="e40bf-105">Duyệt trang web, bấm vào biểu tượng cài đặt, và sau đó bấm **thiết đặt trang web**.</span><span class="sxs-lookup"><span data-stu-id="e40bf-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="e40bf-106">Trong **bộ sưu tập trang web quản trị**, bấm vào **tính năng thu thập trang web**.</span><span class="sxs-lookup"><span data-stu-id="e40bf-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="e40bf-107">Cạnh **chế độ khóa cấp phép người dùng truy cập hạn chế**, nhấp vào **hủy**kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="e40bf-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="e40bf-108">Thông báo truy cập từ chối cũng có thể xảy ra cho cặp chia sẻ nếu trang web xuất bản.</span><span class="sxs-lookup"><span data-stu-id="e40bf-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="e40bf-109">Để biết thông tin, xem [truy cập bị từ chối khi truy cập vào cặp chia sẻ](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="e40bf-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="e40bf-110">Nếu một người có thông báo "truy cập từ chối" khi cố gắng để xem yêu cầu truy cập, người dùng cần phải được thêm vào như là một quản trị viên bộ sưu tập trang web hoặc thành viên của nhóm chủ sở hữu trang web.</span><span class="sxs-lookup"><span data-stu-id="e40bf-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="e40bf-111">Để biết thêm thông tin, xem [truy cập từ chối truy cập yêu cầu danh sách](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="e40bf-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="e40bf-112">Nếu người dùng có thông báo "truy cập từ chối" sau khi họ đã bị xoá khỏi Active Directory tại chỗ và sau đó thêm lại, xem [truy cập bị từ chối khi tài khoản người dùng được đồng bộ hóa với Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="e40bf-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

