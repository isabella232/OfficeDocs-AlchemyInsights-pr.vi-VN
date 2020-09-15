---
title: Khắc phục sự cố Access bị từ chối thư vào các site OneDrive for Business
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670638"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="fd077-102">Khắc phục sự cố Access bị từ chối thư vào các site OneDrive for Business</span><span class="sxs-lookup"><span data-stu-id="fd077-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="fd077-103">Sự cố này thường xảy ra khi người dùng bị xóa bỏ và được tạo lại với cùng tên chính của người dùng (UPN).</span><span class="sxs-lookup"><span data-stu-id="fd077-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="fd077-104">Tài khoản mới được tạo bằng một giá trị PUID khác (ID duy nhất của Passport).</span><span class="sxs-lookup"><span data-stu-id="fd077-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="fd077-105">Khi người dùng cố gắng truy nhập vào một tuyển tập trang hoặc OneDrive của họ, người dùng có một con dấu PUID không chính xác.</span><span class="sxs-lookup"><span data-stu-id="fd077-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="fd077-106">Kịch bản thứ hai liên quan đến việc đồng bộ hóa thư mục với một đơn vị tổ chức Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="fd077-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="fd077-107">Nếu người dùng đã đăng nhập vào SharePoint, sau đó được di chuyển đến OU và resynced khác với SharePoint, họ có thể gặp phải vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="fd077-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="fd077-108">Để giải quyết sự cố này, bạn nên khôi phục UPN ban đầu với các bước trong bài viết, [khôi phục người dùng trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="fd077-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="fd077-109">Nếu bạn không thể khôi phục người dùng ban đầu, bạn nên loại bỏ người dùng cũ khỏi site OneDrive bằng cách sử dụng các bước này, hãy [loại bỏ người dùng khỏi danh sách thông tin người dùng]().</span><span class="sxs-lookup"><span data-stu-id="fd077-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="fd077-110">Sau khi hoàn thành xong, bạn có thể xác nhận người dùng có quyền quản trị đối với site OneDrive bằng cách làm theo các bước để [Thêm người quản trị cho OneDrive của người dùng](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="fd077-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="fd077-111">Để biết thêm thông tin về các mức cấp phép, hãy xem bài viết, [Tìm hiểu các mức cấp phép trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="fd077-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
