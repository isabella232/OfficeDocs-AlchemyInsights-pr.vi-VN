---
title: Tạo site SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786587"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="32a04-102">Tạo site SharePoint</span><span class="sxs-lookup"><span data-stu-id="32a04-102">Create a SharePoint site</span></span>

<span data-ttu-id="32a04-103">Tạo hoặc quản lý các site từ [các site hiện hoạt](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) trong Trung tâm quản trị SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32a04-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="32a04-104">Để biết thêm thông tin, hãy xem [quản lý site trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="32a04-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="32a04-105">Ý</span><span class="sxs-lookup"><span data-stu-id="32a04-105">Tips:</span></span>

- <span data-ttu-id="32a04-106">Bạn **không thể** tạo site có cùng một URL của site hiện có.</span><span class="sxs-lookup"><span data-stu-id="32a04-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="32a04-107">Nếu bạn đã xóa một site và muốn sử dụng lại URL, nó có thể là site đã xóa vẫn tồn tại trong [các site đã xóa](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="32a04-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="32a04-108">Site sẽ cần bị xóa vĩnh viễn để dùng lại URL.</span><span class="sxs-lookup"><span data-stu-id="32a04-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="32a04-109">Để loại bỏ hoàn toàn một site với PowerShell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="32a04-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="32a04-110">Một số người dùng có thể không thể tạo trang.</span><span class="sxs-lookup"><span data-stu-id="32a04-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="32a04-111">[Xem mục quản lý việc tạo site trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="32a04-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="32a04-112">Trang web có thể có vẻ khó khăn khi **tạo** lâu hơn dự kiến.</span><span class="sxs-lookup"><span data-stu-id="32a04-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="32a04-113">Nếu đã trôi qua 24 giờ kể từ lần đầu tiên bạn gặp sự cố này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="32a04-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="32a04-114">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="32a04-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="32a04-115">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn tất một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="32a04-115">Please give us at least 24 hours to complete a solution.</span></span>
