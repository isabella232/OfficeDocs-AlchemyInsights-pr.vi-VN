---
title: Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 5a1cdeefa4474e8ce0e6a7a37be016cc87b9791d
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498036"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="0f73b-102">Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="0f73b-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="0f73b-p101">Nếu một trang web OneDrive hoặc SharePoint không phải là có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ. [Kiểm tra bảng điều khiển dịch vụ sức khỏe](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="0f73b-p101">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue. [Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth)</span></span>
  
<span data-ttu-id="0f73b-p102">Nếu bạn muốn mọi người trong tổ chức của bạn để có thể đăng nhập và sử dụng SharePoint và OneDrive, bạn cần phải thêm tài khoản cho họ và đảm bảo rằng họ có một giấy phép cho phép họ truy cập SharePoint và OneDrive. Cách dễ nhất để thêm người dùng là ở trung tâm quản trị Office 365.</span><span class="sxs-lookup"><span data-stu-id="0f73b-p102">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive. The easiest way to add users is in the Office 365 admin center.</span></span>
  
1. <span data-ttu-id="0f73b-107">Đi vào [hoạt động người dùng trang trong Trung tâm quản trị Office 365](https://portal.office.com/adminportal/home#/users), và sau đó nhấp vào **Thêm người dùng**.</span><span class="sxs-lookup"><span data-stu-id="0f73b-107">Go to the [Active users page in the Office 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="0f73b-108">Điền các thông tin cho người dùng, và chắc chắn rằng dưới **giấy phép sản phẩm**, một giấy phép được gán và **SharePoint Online** được chọn.</span><span class="sxs-lookup"><span data-stu-id="0f73b-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="0f73b-p103">Lưu ý rằng nếu bạn cho phép bên ngoài chia sẻ trong tổ chức của bạn, người dùng có thể chia sẻ nội dung SharePoint và OneDrive với những người bên ngoài tổ chức. Bạn không cần phải cung cấp cho các giấy phép người dùng bên ngoài. Bạn cũng không cần phải thêm tài khoản cho họ, trừ khi chia sẻ được thiết lập để "Duy nhất hiện tại người dùng bên ngoài." Trong trường hợp đó, nếu người dân không trong tổ chức của bạn thư mục, bạn cần phải thêm họ làm người dùng đánh trong Trung tâm quản trị quảng cáo Azure.</span><span class="sxs-lookup"><span data-stu-id="0f73b-p103">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization. You don't need to give these external users licenses. You also don't need to add accounts for them, unless sharing is set to "Only existing external users." In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

