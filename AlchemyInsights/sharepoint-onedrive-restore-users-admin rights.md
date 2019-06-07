---
title: Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a689769dab24e12832ddc0937bc5ddc3d71dbee3
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759277"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="a700c-102">Cung cấp cho người dùng quyền truy cập cho SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="a700c-102">Give users access to SharePoint and OneDrive</span></span>

<span data-ttu-id="a700c-103">Vấn đề này thường xảy ra khi người dùng xóa và tạo lại với cùng tên người dùng chính (UPN).</span><span class="sxs-lookup"><span data-stu-id="a700c-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="a700c-104">Tài khoản mới được tạo ra bằng cách sử dụng một giá trị PUID (hộ chiếu duy nhất ID) khác nhau.</span><span class="sxs-lookup"><span data-stu-id="a700c-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="a700c-105">Khi người dùng cố gắng truy cập vào một bộ sưu tập trang web hoặc OneDrive của họ, người dùng có một PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="a700c-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="a700c-106">Một kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức hoạt động Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="a700c-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="a700c-107">Nếu người dùng đã đăng nhập vào SharePoint, và sau đó được chuyển đến một OU khác nhau và resynced với SharePoint, họ có thể gặp vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="a700c-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="a700c-108">Để giải quyết vấn đề này, bạn nên khôi phục lại các UPN ban đầu với các bước trong bài viết,[khôi phục người dùng trong Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a700c-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="a700c-109">Sau khi điều này được thực hiện, bạn có thể xác thực người dùng có quyền quản trị trang web OneDrive bằng cách làm theo các bước để [Thêm admin của cho một người sử dụng OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="a700c-109">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="a700c-110">Để biết thêm chi tiết về mức độ cho phép, hãy xem bài viết, [sự hiểu biết cho phép cấp trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a700c-110">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
