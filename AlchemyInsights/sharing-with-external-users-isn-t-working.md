---
title: Chia sẻ với người dùng bên ngoài không hoạt động
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 700e6d24e49cf11bf91780895f5a796cc1d8349d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753448"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="36baf-102">Sửa chữa các vấn đề về chia sẻ nội dung SharePoint với người dùng bên ngoài</span><span class="sxs-lookup"><span data-stu-id="36baf-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="36baf-103">Đảm bảo rằng bên ngoài chia sẻ được bật cho tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="36baf-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="36baf-104">Đi đến các [dịch vụ &amp; add-in trang trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), và nhấp vào **các trang web**.</span><span class="sxs-lookup"><span data-stu-id="36baf-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="36baf-105">Đảm bảo rằng các thiết lập được bật "On."</span><span class="sxs-lookup"><span data-stu-id="36baf-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="36baf-106">Nếu "Chỉ người dùng bên ngoài hiện tại" được chọn, hãy chắc chắn rằng người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="36baf-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="36baf-107">Đảm bảo rằng ngoài việc chia sẻ nó bật lên cho trang web.</span><span class="sxs-lookup"><span data-stu-id="36baf-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="36baf-108">Đối với một bộ sưu tập cổ điển trang web:</span><span class="sxs-lookup"><span data-stu-id="36baf-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="36baf-109">Trong Trung tâm quản trị cổ điển SharePoint, trong ngăn bên trái, nhấp vào **các bộ sưu tập trang web**.</span><span class="sxs-lookup"><span data-stu-id="36baf-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="36baf-110">Chọn các trang web hoặc các trang web và trên các ribbon, hãy nhấp vào **chia sẻ**.</span><span class="sxs-lookup"><span data-stu-id="36baf-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="36baf-111">Cho một trang web đội thuộc về một nhóm Office 365, hoặc một trang web thông tin liên lạc:</span><span class="sxs-lookup"><span data-stu-id="36baf-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="36baf-112">Các loại trang web mới có chia sẻ cùng cài đặt như thiết lập trên toàn tổ chức của bạn, trừ khi thiết lập phạm vi tổ chức cho phép chia sẻ tập tin bằng cách sử dụng liên kết mà không cần đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="36baf-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="36baf-113">Trong trường hợp này, các trang web cho phép chia sẻ với các mới và hiện tại bên ngoài người dùng đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="36baf-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="36baf-114">Để thay đổi các thiết lập cho trang web cụ thể, sử dụng trung tâm quản trị SharePoint mới (xem trước) hoặc PowerShell.</span><span class="sxs-lookup"><span data-stu-id="36baf-114">To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell.</span></span> <span data-ttu-id="36baf-115">[Tìm hiểu thêm](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="36baf-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="36baf-116">Cài đặt chia sẻ bên ngoài cho bất kỳ trang web có thể hạn chế hơn so với các thiết lập toàn tổ chức của bạn, nhưng không nhiều hơn permissive hơn thiết đặt phạm vi tổ chức.</span><span class="sxs-lookup"><span data-stu-id="36baf-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

