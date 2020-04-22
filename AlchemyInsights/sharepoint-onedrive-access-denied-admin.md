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
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758546"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="1dcaa-102">Khắc phục sự cố truy cập từ chối thư trong SharePoint/OneDrive quản trị Trung tâm</span><span class="sxs-lookup"><span data-stu-id="1dcaa-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="1dcaa-103">Nếu bạn nhận được thông báo từ chối truy cập khi cố gắng duyệt tới Trung tâm quản trị SharePoint/OneDrive, hãy đảm bảo rằng bạn [gán giấy phép cho người dùng](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="1dcaa-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="1dcaa-104">Nếu người dùng có giấy phép, bạn cũng nên chắc chắn rằng họ được [gán một vai trò người quản trị](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) có thể truy cập các trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="1dcaa-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="1dcaa-105">Vấn đề này cũng có thể xảy ra khi người dùng bị xoá và tạo lại với cùng tên người dùng chính (UPN).</span><span class="sxs-lookup"><span data-stu-id="1dcaa-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="1dcaa-106">Tài khoản mới được tạo ra bằng cách sử dụng giá trị PUID (Passport Unique ID) khác nhau.</span><span class="sxs-lookup"><span data-stu-id="1dcaa-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="1dcaa-107">Khi người dùng cố gắng truy cập vào bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="1dcaa-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="1dcaa-108">Trường hợp thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="1dcaa-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="1dcaa-109">Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một đơn vị tổ chức khác và resynced với SharePoint, họ có thể gặp phải sự cố này.</span><span class="sxs-lookup"><span data-stu-id="1dcaa-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="1dcaa-110">Để giải quyết vấn đề này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1dcaa-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="1dcaa-111">Lưu ý: nếu một trung tâm quản trị OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng trước đây đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="1dcaa-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="1dcaa-112">[Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="1dcaa-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


