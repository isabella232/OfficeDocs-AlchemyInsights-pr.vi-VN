---
title: Tạo một trang web SharePoint
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 92bb7b5f0a684936db52f6be9e00c8dff3378bb5
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657525"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="a14a4-102">Tạo một trang web SharePoint</span><span class="sxs-lookup"><span data-stu-id="a14a4-102">Create a SharePoint site</span></span>

<span data-ttu-id="a14a4-p101">Xem [các trang web quản lý trong Trung tâm quản trị mới của SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation ) cho các trang web sáng tạo tùy chọn. Chọn để tạo ra một [nhóm trang web](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (mà sẽ tạo ra một nhóm Office 365) hoặc một [trang web thông tin liên lạc](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Để tạo một [trang web cổ điển](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), hoặc một trang web mới đội không bao gồm một nhóm Office 365, bấm vào **tuỳ chọn khác**.</span><span class="sxs-lookup"><span data-stu-id="a14a4-p101">See [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation ) for site creation options. Select to create a [team site](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US) (which will create an Office 365 group) or a [communication site](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). To create a [classic site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site), or a new team site that doesn't include an Office 365 group, click **Other options**.</span></span> 
  
<span data-ttu-id="a14a4-106">Lời khuyên:</span><span class="sxs-lookup"><span data-stu-id="a14a4-106">Tips:</span></span>
- <span data-ttu-id="a14a4-107">*Bạn không thể tạo ra một trang web với cùng một URL của một trang web hiện có. Nếu bạn xóa một trang web và có nhu cầu tái sử dụng URL, nó có thể đã bị xóa trang web vẫn còn tồn tại trong **các trang web đã bị xoá**. Để quản lý đã xoá cho xem các trang web, [xóa một trang web](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). Để hoàn toàn loại bỏ một trang web bằng Powershell, hãy xem ví dụ lệnh ghép ngắn [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .*</span><span class="sxs-lookup"><span data-stu-id="a14a4-107">*You cannot create a site with the same URL of an existing site. If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**. To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site). To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.*</span></span>
- <span data-ttu-id="a14a4-108">*Một số người dùng không thể tạo ra một trang web. Hãy xem [quản lý tạo ra trang web trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span><span class="sxs-lookup"><span data-stu-id="a14a4-108">*Some users may not be able to create a site. See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).*</span></span>
- <span data-ttu-id="a14a4-109">*Nó có thể trang web xuất hiện khó khăn lúc **tạo** dài hơn dự kiến. Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn lần đầu tiên thấy vấn đề này, xin vui lòng đăng nhập một vé hỗ trợ. Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp. Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.*</span><span class="sxs-lookup"><span data-stu-id="a14a4-109">*It's possible the site appears stuck at **Creating** longer than expected. If more than 24 hours have passed since you first saw this issue, please log a support ticket. In many cases, we're already working on a solution. Please give us at least 24 hours to complete a solution.*</span></span>
