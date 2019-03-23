---
title: Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: ebb9037362d261b81b9b1dcafcbe461aac7f4963
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759640"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="7c2c9-102">Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="7c2c9-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="7c2c9-103">Nếu một trang web OneDrive hoặc SharePoint không phải là có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="7c2c9-104">Kiểm tra bảng điều khiển dịch vụ sức khỏe</span><span class="sxs-lookup"><span data-stu-id="7c2c9-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="7c2c9-105">Nếu bạn muốn mọi người trong tổ chức của bạn để có thể đăng nhập và sử dụng SharePoint và OneDrive, bạn cần phải thêm tài khoản cho họ và đảm bảo rằng họ có một giấy phép cho phép họ truy cập SharePoint và OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="7c2c9-106">Cách dễ nhất để thêm người dùng là ở trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="7c2c9-107">Đi đến [trang Trung tâm quản trị Microsoft 365 người dùng hoạt động](https://portal.office.com/adminportal/home#/users), và sau đó nhấp vào **Thêm người dùng**.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="7c2c9-108">Điền các thông tin cho người dùng, và chắc chắn rằng dưới **giấy phép sản phẩm**, một giấy phép được gán và **SharePoint Online** được chọn.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="7c2c9-109">Lưu ý rằng nếu bạn cho phép bên ngoài chia sẻ trong tổ chức của bạn, người dùng có thể chia sẻ nội dung SharePoint và OneDrive với những người bên ngoài tổ chức.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="7c2c9-110">Bạn không cần phải cung cấp cho các giấy phép người dùng bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="7c2c9-111">Bạn cũng không cần phải thêm tài khoản cho họ, trừ khi chia sẻ được thiết lập để "Duy nhất hiện tại người dùng bên ngoài."</span><span class="sxs-lookup"><span data-stu-id="7c2c9-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="7c2c9-112">Trong trường hợp đó, nếu người dân không trong tổ chức của bạn thư mục, bạn cần phải thêm họ làm người dùng đánh trong Trung tâm quản trị quảng cáo Azure.</span><span class="sxs-lookup"><span data-stu-id="7c2c9-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

