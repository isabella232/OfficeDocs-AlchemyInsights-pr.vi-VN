---
title: Chia sẻ với người dùng bên ngoài không hoạt động
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913024"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="b43f3-102">Khắc phục sự cố chia sẻ nội dung SharePoint với người dùng bên ngoài</span><span class="sxs-lookup"><span data-stu-id="b43f3-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="b43f3-103">Đảm bảo rằng việc chia sẻ bên ngoài được bật cho tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="b43f3-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="b43f3-104">Truy cập [trang dịch &amp; vụ bổ sung trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)và nhấp vào **trang web**.</span><span class="sxs-lookup"><span data-stu-id="b43f3-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="b43f3-105">Đảm bảo rằng cài đặt được bật thành "bật".</span><span class="sxs-lookup"><span data-stu-id="b43f3-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="b43f3-106">Nếu "chỉ người dùng bên ngoài hiện tại" được chọn, đảm bảo rằng người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b43f3-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="b43f3-107">Hãy chắc chắn rằng chia sẻ bên ngoài nó bật cho trang web.</span><span class="sxs-lookup"><span data-stu-id="b43f3-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="b43f3-108">Đối với bộ sưu tập trang web cổ điển:</span><span class="sxs-lookup"><span data-stu-id="b43f3-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="b43f3-109">Trong Trung tâm quản trị SharePoint mới, trong ngăn bên trái, bấm vào **các trang web**.</span><span class="sxs-lookup"><span data-stu-id="b43f3-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="b43f3-110">Chọn trang web hoặc trang web và trên ruy băng, bấm vào **chia sẻ**.</span><span class="sxs-lookup"><span data-stu-id="b43f3-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="b43f3-111">Trang web nhóm thuộc một nhóm Microsoft 365 hoặc một trang web liên lạc:</span><span class="sxs-lookup"><span data-stu-id="b43f3-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="b43f3-112">Các loại trang web mới này có cài đặt chia sẻ tương tự như cài đặt trên toàn tổ chức, trừ khi cài đặt trên toàn tổ chức cho phép chia sẻ tệp bằng cách sử dụng liên kết không yêu cầu đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="b43f3-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="b43f3-113">Trong trường hợp này, các trang web cho phép chia sẻ với người dùng bên ngoài mới và hiện có đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="b43f3-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="b43f3-114">Để thay đổi cài đặt cho các trang web cụ thể, sử dụng trung tâm quản trị SharePoint mới hoặc PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b43f3-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="b43f3-115">Tìm hiểu [Thêm](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="b43f3-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="b43f3-116">Cài đặt chia sẻ bên ngoài cho bất kỳ trang web nào có thể hạn chế hơn so với cài đặt trong phạm vi tổ chức của bạn, nhưng không có sự cho phép hơn so với cài đặt trên toàn tổ chức.</span><span class="sxs-lookup"><span data-stu-id="b43f3-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

