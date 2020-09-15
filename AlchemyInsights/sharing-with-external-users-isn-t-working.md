---
title: Chia sẻ với người dùng bên ngoài không hoạt động
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691597"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="cbeab-102">Khắc phục sự cố chia sẻ nội dung SharePoint với người dùng bên ngoài</span><span class="sxs-lookup"><span data-stu-id="cbeab-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="cbeab-103">Đảm bảo chia sẻ bên ngoài được bật cho tổ chức của bạn:</span><span class="sxs-lookup"><span data-stu-id="cbeab-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="cbeab-104">Đi đến [trang bổ trợ dịch vụ &amp; trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), rồi bấm vào **site**.</span><span class="sxs-lookup"><span data-stu-id="cbeab-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="cbeab-105">Đảm bảo cài đặt được bật thành "bật."</span><span class="sxs-lookup"><span data-stu-id="cbeab-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="cbeab-106">Nếu "chỉ những người dùng bên ngoài hiện có" được chọn, hãy đảm bảo rằng người dùng bên ngoài được liệt kê trong Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cbeab-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="cbeab-107">Đảm bảo chia sẻ bên ngoài nó bật đối với trang.</span><span class="sxs-lookup"><span data-stu-id="cbeab-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="cbeab-108">Đối với tuyển tập trang cổ điển:</span><span class="sxs-lookup"><span data-stu-id="cbeab-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="cbeab-109">Trong Trung tâm quản trị SharePoint mới, trong ngăn bên trái, hãy bấm **site**.</span><span class="sxs-lookup"><span data-stu-id="cbeab-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="cbeab-110">Chọn trang hoặc site và trên Ribbon, bấm **chia sẻ**.</span><span class="sxs-lookup"><span data-stu-id="cbeab-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="cbeab-111">Đối với một site nhóm thuộc nhóm Microsoft 365 hoặc một site liên lạc:</span><span class="sxs-lookup"><span data-stu-id="cbeab-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="cbeab-112">Những loại site mới này có cùng thiết đặt chia sẻ như thiết đặt toàn bộ tổ chức của bạn, trừ khi thiết đặt toàn bộ tổ chức cho phép chia sẻ tệp bằng các liên kết không yêu cầu đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="cbeab-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="cbeab-113">Trong trường hợp này, các site cho phép chia sẻ với những người dùng bên ngoài mới và hiện có đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="cbeab-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="cbeab-114">Để thay đổi thiết đặt cho các site cụ thể, hãy sử dụng trung tâm quản trị SharePoint mới hoặc PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cbeab-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="cbeab-115">[Tìm hiểu thêm](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="cbeab-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cbeab-116">Thiết đặt chia sẻ bên ngoài cho bất kỳ trang nào có thể được thêm hạn chế so với cài đặt phạm vi tổ chức của bạn, nhưng không được nhiều hơn so với cài đặt phạm vi tổ chức.</span><span class="sxs-lookup"><span data-stu-id="cbeab-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

