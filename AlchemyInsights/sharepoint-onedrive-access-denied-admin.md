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
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707976"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="aa1ae-102">Khắc phục sự cố truy nhập bị từ chối thư trong Trung tâm quản trị SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="aa1ae-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="aa1ae-103">Nếu bạn nhận được một truy nhập bị từ chối thư khi tìm cách duyệt đến Trung tâm quản trị SharePoint/OneDrive, hãy đảm bảo rằng bạn [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="aa1ae-104">Nếu người dùng có giấy phép, bạn cũng nên đảm bảo rằng chúng được [gán vai trò người quản trị](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) có thể truy nhập vào Trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="aa1ae-105">Sự cố này cũng có thể xảy ra khi người dùng bị xóa bỏ và được tạo lại với cùng tên chính của người dùng (UPN).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="aa1ae-106">Tài khoản mới được tạo bằng một giá trị PUID khác (ID duy nhất của Passport).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="aa1ae-107">Khi người dùng cố gắng truy nhập vào một tuyển tập trang hoặc OneDrive của họ, người dùng có một con dấu PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="aa1ae-108">Kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="aa1ae-109">Nếu người dùng đã đăng nhập vào SharePoint, sau đó được di chuyển đến OU và resynced khác với SharePoint, họ có thể gặp phải vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="aa1ae-110">Để giải quyết sự cố này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="aa1ae-111">Lưu ý: nếu Trung tâm quản trị OneDrive hoặc SharePoint không sẵn dùng cho nhiều người dùng trước đây có quyền truy nhập, thì có thể có sự cố dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="aa1ae-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="aa1ae-112">[Kiểm tra bảng điều khiển trạng thái dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="aa1ae-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


