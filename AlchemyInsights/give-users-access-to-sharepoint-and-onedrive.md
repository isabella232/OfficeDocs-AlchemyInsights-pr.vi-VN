---
title: Cấp cho người dùng quyền truy nhập vào SharePoint và OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677229"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="aa753-102">Cấp cho người dùng quyền truy nhập vào SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="aa753-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="aa753-103">Nếu một site OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, có thể có sự cố dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="aa753-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="aa753-104">Kiểm tra bảng điều khiển trạng thái dịch vụ</span><span class="sxs-lookup"><span data-stu-id="aa753-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="aa753-105">Nếu bạn muốn mọi người trong tổ chức của bạn có thể đăng nhập và sử dụng SharePoint và OneDrive, bạn cần thêm tài khoản cho họ và đảm bảo rằng họ có giấy phép cung cấp cho họ quyền truy nhập vào SharePoint và OneDrive.</span><span class="sxs-lookup"><span data-stu-id="aa753-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="aa753-106">Cách dễ nhất để thêm người dùng trong Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="aa753-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="aa753-107">Đi đến [trang người dùng hiện hoạt trong Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/users), rồi bấm **Thêm người dùng**.</span><span class="sxs-lookup"><span data-stu-id="aa753-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="aa753-108">Điền thông tin cho người dùng và đảm bảo rằng bên dưới **giấy phép sản phẩm**, giấy phép được gán và **SharePoint Online** được chọn.</span><span class="sxs-lookup"><span data-stu-id="aa753-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="aa753-109">Lưu ý rằng nếu bạn cho phép chia sẻ bên ngoài trong tổ chức của mình, người dùng có thể chia sẻ nội dung SharePoint và OneDrive với những người bên ngoài tổ chức.</span><span class="sxs-lookup"><span data-stu-id="aa753-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="aa753-110">Bạn không cần phải cung cấp cho những giấy phép người dùng bên ngoài này.</span><span class="sxs-lookup"><span data-stu-id="aa753-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="aa753-111">Bạn cũng không cần phải thêm tài khoản cho họ, trừ khi chia sẻ được đặt là "chỉ những người dùng bên ngoài hiện có."</span><span class="sxs-lookup"><span data-stu-id="aa753-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="aa753-112">Trong trường hợp đó, nếu mọi người không có trong danh bạ của tổ chức bạn, bạn cần thêm chúng làm người dùng khách trong Trung tâm quản trị Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aa753-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

