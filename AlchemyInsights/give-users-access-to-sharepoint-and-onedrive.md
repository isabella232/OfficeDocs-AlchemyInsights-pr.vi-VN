---
title: Cấp cho người dùng quyền truy cập vào SharePoint và OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: eead51d6d16206de19bca213d6df72dbb6b66c8b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051951"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="7c6fc-102">Cấp cho người dùng quyền truy cập vào SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c6fc-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="7c6fc-103">Nếu một trang web OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="7c6fc-104">Kiểm tra bảng điều khiển tình trạng dịch vụ</span><span class="sxs-lookup"><span data-stu-id="7c6fc-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="7c6fc-105">Nếu bạn muốn những người trong tổ chức của bạn có thể đăng nhập và sử dụng SharePoint và OneDrive, bạn cần phải thêm tài khoản cho họ và đảm bảo rằng họ có giấy phép cung cấp cho họ quyền truy cập vào SharePoint và OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="7c6fc-106">Cách dễ nhất để thêm người dùng nằm trong Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="7c6fc-107">Truy cập [trang người dùng đang hoạt động trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/users), và sau đó nhấp vào **Thêm người dùng**.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="7c6fc-108">Điền thông tin cho người dùng và đảm bảo rằng theo giấy phép **sản phẩm**, giấy phép được chỉ định và **SharePoint trực tuyến** được chọn.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="7c6fc-109">Lưu ý rằng nếu bạn cho phép chia sẻ bên ngoài trong tổ chức của mình, người dùng có thể chia sẻ nội dung SharePoint và OneDrive với những người bên ngoài tổ chức.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="7c6fc-110">Bạn không cần phải cung cấp cho các giấy phép người dùng bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="7c6fc-111">Bạn cũng không cần phải thêm tài khoản cho họ, trừ khi chia sẻ được đặt thành "chỉ người dùng bên ngoài hiện tại."</span><span class="sxs-lookup"><span data-stu-id="7c6fc-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="7c6fc-112">Trong trường hợp đó, nếu những người không có trong thư mục của tổ chức của bạn, bạn cần phải thêm họ làm người dùng khách trong Trung tâm quản trị Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7c6fc-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

