---
title: Tạo một trang web SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738219"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="490b6-102">Tạo một trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="490b6-102">Create a SharePoint site</span></span>

<span data-ttu-id="490b6-103">Bạn có thể xem những thông tin sau để tạo trang web SharePoint:</span><span class="sxs-lookup"><span data-stu-id="490b6-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="490b6-104">[Quản lý trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-site-creation): tìm hiểu về các tùy chọn tạo trang web, bao gồm cách tạo trang web cổ điển hoặc trang web nhóm không bao gồm nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="490b6-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="490b6-105">[Tạo một trang web nhóm trong SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): tìm hiểu cách tạo trang web nhóm.</span><span class="sxs-lookup"><span data-stu-id="490b6-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="490b6-106">[Tạo một trang web liên lạc trong SharePoint trực tuyến](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): tìm hiểu cách tạo một trang web liên lạc.</span><span class="sxs-lookup"><span data-stu-id="490b6-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="490b6-107">[Quản lý trang web trong Trung tâm quản trị SharePoint mới](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): tìm hiểu cách tạo một trang web cổ điển hoặc một trang web nhóm không bao gồm một nhóm Office 365.</span><span class="sxs-lookup"><span data-stu-id="490b6-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="490b6-108">[! Mẹo</span><span class="sxs-lookup"><span data-stu-id="490b6-108">[!Tips]</span></span>
> - <span data-ttu-id="490b6-109">Bạn không thể tạo một trang web có cùng URL của trang web hiện có.</span><span class="sxs-lookup"><span data-stu-id="490b6-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="490b6-110">Nếu bạn đã xóa một trang web và muốn sử dụng lại URL, có thể trang web đã xóa vẫn tồn tại trong **các trang web đã xóa**.</span><span class="sxs-lookup"><span data-stu-id="490b6-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="490b6-111">Để quản lý các trang web đã xóa, xem, [xóa một trang web](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="490b6-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="490b6-112">Để loại bỏ hoàn toàn một trang web với PowerShell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="490b6-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="490b6-113">Một số người dùng có thể không thể tạo một trang web.</span><span class="sxs-lookup"><span data-stu-id="490b6-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="490b6-114">Xem [quản lý tạo trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="490b6-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="490b6-115">Có thể trang web xuất hiện bị kẹt lúc **tạo** lâu hơn dự kiến.</span><span class="sxs-lookup"><span data-stu-id="490b6-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="490b6-116">Nếu hơn 24 giờ đã trôi qua kể từ lần đầu tiên bạn thấy vấn đề này, vui lòng đăng nhập một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="490b6-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="490b6-117">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="490b6-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="490b6-118">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="490b6-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="490b6-119">Nếu bạn cần tạo một trang web nhóm mới không bao gồm một nhóm Office 365,</span><span class="sxs-lookup"><span data-stu-id="490b6-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


