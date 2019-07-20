---
title: Tạo một trang web SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802988"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="1b215-102">Tạo một trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="1b215-102">Create a SharePoint site</span></span>

<span data-ttu-id="1b215-103">Bạn có thể thấy sau đây để biết thông tin về SharePoint trang web tạo ra:</span><span class="sxs-lookup"><span data-stu-id="1b215-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="1b215-104">[Quản lý các trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation): tìm hiểu về lựa chọn sáng tạo trang web, bao gồm làm thế nào để tạo một trang web cổ điển hoặc một trang web đội không bao gồm một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="1b215-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="1b215-105">[Tạo một nhóm trang web trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): tìm hiểu làm thế nào để tạo một trang web đội ngũ.</span><span class="sxs-lookup"><span data-stu-id="1b215-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="1b215-106">[Tạo một trang web thông tin liên lạc trong SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): tìm hiểu làm thế nào để tạo một trang web thông tin liên lạc.</span><span class="sxs-lookup"><span data-stu-id="1b215-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="1b215-107">[Quản lý các trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): tìm hiểu làm thế nào để tạo một trang web cổ điển hoặc một trang web đội không bao gồm một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="1b215-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Lời khuyên]
> - <span data-ttu-id="1b215-109">Bạn không thể tạo ra một trang web với cùng một URL của một trang web hiện có.</span><span class="sxs-lookup"><span data-stu-id="1b215-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="1b215-110">Nếu bạn xóa một trang web và có nhu cầu tái sử dụng URL, nó có thể đã bị xóa trang web vẫn còn tồn tại trong **các trang web đã bị xoá**.</span><span class="sxs-lookup"><span data-stu-id="1b215-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="1b215-111">Để quản lý đã xoá cho xem các trang web, [xóa một trang web](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="1b215-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="1b215-112">Để hoàn toàn loại bỏ một trang web bằng Powershell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="1b215-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="1b215-113">Một số người dùng không thể tạo ra một trang web.</span><span class="sxs-lookup"><span data-stu-id="1b215-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="1b215-114">Hãy xem [quản lý tạo ra trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="1b215-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="1b215-115">Nó có thể trang web xuất hiện khó khăn lúc **tạo** dài hơn dự kiến.</span><span class="sxs-lookup"><span data-stu-id="1b215-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="1b215-116">Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="1b215-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1b215-117">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="1b215-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1b215-118">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="1b215-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="1b215-119">Nếu bạn cần để tạo ra một trang web mới của đội tuyển mà không bao gồm một nhóm Office 365,</span><span class="sxs-lookup"><span data-stu-id="1b215-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


