---
title: Tạo một trang web SharePoint
ms.author: pebaum
author: todmccoy
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
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770877"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="4ac51-102">Tạo một trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="4ac51-102">Create a SharePoint site</span></span>

<span data-ttu-id="4ac51-103">Tạo hoặc quản lý trang web từ các [trang web hiện hoạt](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) trong Trung tâm quản trị SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4ac51-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="4ac51-104">Để biết thêm thông tin, hãy xem [quản lý trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4ac51-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="4ac51-105">Mẹo:</span><span class="sxs-lookup"><span data-stu-id="4ac51-105">Tips:</span></span>

- <span data-ttu-id="4ac51-106">Bạn **không thể** tạo một trang web có cùng URL của trang web hiện có.</span><span class="sxs-lookup"><span data-stu-id="4ac51-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="4ac51-107">Nếu bạn đã xóa một trang web và muốn sử dụng lại URL, có thể trang web đã xóa vẫn tồn tại trong [các trang web đã xóa](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="4ac51-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="4ac51-108">Trang web sẽ cần phải được xóa vĩnh viễn để tái sử dụng URL.</span><span class="sxs-lookup"><span data-stu-id="4ac51-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="4ac51-109">Để loại bỏ hoàn toàn một trang web với PowerShell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="4ac51-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="4ac51-110">Một số người dùng có thể không thể tạo một trang web.</span><span class="sxs-lookup"><span data-stu-id="4ac51-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="4ac51-111">[Xem quản lý tạo trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="4ac51-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="4ac51-112">Có thể trang web xuất hiện bị kẹt lúc **tạo** lâu hơn dự kiến.</span><span class="sxs-lookup"><span data-stu-id="4ac51-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="4ac51-113">Nếu hơn 24 giờ đã trôi qua kể từ lần đầu tiên bạn thấy vấn đề này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="4ac51-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4ac51-114">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="4ac51-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4ac51-115">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="4ac51-115">Please give us at least 24 hours to complete a solution.</span></span>
