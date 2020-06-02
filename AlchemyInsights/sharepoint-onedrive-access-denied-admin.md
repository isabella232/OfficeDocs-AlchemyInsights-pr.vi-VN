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
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505401"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="68d42-102">Khắc phục sự cố truy cập từ chối thư trong SharePoint/OneDrive quản trị Trung tâm</span><span class="sxs-lookup"><span data-stu-id="68d42-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="68d42-103">Nếu bạn nhận được thông báo từ chối truy cập khi cố gắng duyệt tới Trung tâm quản trị SharePoint/OneDrive, hãy đảm bảo rằng bạn [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="68d42-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="68d42-104">Nếu người dùng có giấy phép, bạn cũng nên chắc chắn rằng họ được [gán một vai trò người quản trị](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) có thể truy cập các trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="68d42-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="68d42-105">Vấn đề này cũng có thể xảy ra khi người dùng bị xoá và tạo lại với cùng tên người dùng chính (UPN).</span><span class="sxs-lookup"><span data-stu-id="68d42-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="68d42-106">Tài khoản mới được tạo ra bằng cách sử dụng giá trị PUID (Passport Unique ID) khác nhau.</span><span class="sxs-lookup"><span data-stu-id="68d42-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="68d42-107">Khi người dùng cố gắng truy cập vào bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="68d42-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="68d42-108">Trường hợp thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="68d42-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="68d42-109">Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một đơn vị tổ chức khác và resynced với SharePoint, họ có thể gặp phải sự cố này.</span><span class="sxs-lookup"><span data-stu-id="68d42-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="68d42-110">Để giải quyết vấn đề này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="68d42-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="68d42-111">Lưu ý: nếu một trung tâm quản trị OneDrive hoặc SharePoint không có sẵn cho nhiều người dùng trước đây đã có quyền truy cập, có thể có một vấn đề dịch vụ tạm thời.</span><span class="sxs-lookup"><span data-stu-id="68d42-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="68d42-112">[Kiểm tra bảng điều khiển tình trạng dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="68d42-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


