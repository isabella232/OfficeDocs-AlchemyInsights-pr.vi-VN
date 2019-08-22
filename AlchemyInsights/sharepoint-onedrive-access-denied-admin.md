---
title: Khắc phục sự cố truy cập từ chối các thư
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503570"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="8dfee-102">Khắc phục sự cố truy cập từ chối các thư trong Trung tâm quản trị Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="8dfee-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="8dfee-103">Nếu bạn nhận được quyền truy cập bị từ chối thư khi cố gắng để duyệt đến một trung tâm quản trị Sharepoint/OneDrive, hãy chắc chắn rằng bạn [gán một giấy phép cho người dùng](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="8dfee-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="8dfee-104">Nếu người dùng có một giấy phép, bạn cũng nên chắc chắn họ là [được gán vai trò người quản trị](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) mà có thể truy cập Trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="8dfee-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="8dfee-105">Vấn đề này cũng có thể xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN).</span><span class="sxs-lookup"><span data-stu-id="8dfee-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="8dfee-106">Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau.</span><span class="sxs-lookup"><span data-stu-id="8dfee-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="8dfee-107">Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="8dfee-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="8dfee-108">Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="8dfee-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="8dfee-109">Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="8dfee-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="8dfee-110">Để giải quyết vấn đề này, bạn nên khôi phục lại UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="8dfee-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="8dfee-111">Lưu ý: Nếu một trung tâm OneDrive hoặc SharePoint Admin là không có sẵn cho nhiều người dùng trước đó đã truy cập, có thể có một vấn đề tạm thời dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="8dfee-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="8dfee-112">[Kiểm tra bảng điều khiển dịch vụ y tế](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="8dfee-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


