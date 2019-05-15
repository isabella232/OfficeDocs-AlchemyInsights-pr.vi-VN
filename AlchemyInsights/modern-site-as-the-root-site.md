---
title: Các trang web hiện đại như các trang web gốc
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057799"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="cbc79-102">Các trang web hiện đại như là trang web gốc</span><span class="sxs-lookup"><span data-stu-id="cbc79-102">Modern site as root site</span></span>

<span data-ttu-id="cbc79-103">[Mục tiêu phát hành](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) khách có thể bây giờ cho phép trải nghiệm trang web truyền thông hiện đại tại trang web gốc cổ điển của người thuê nhà của SharePoint.</span><span class="sxs-lookup"><span data-stu-id="cbc79-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="cbc79-104">Tính năng này có thể được kích hoạt bằng cách chạy một lệnh ghép ngắn PowerShell đơn giản.</span><span class="sxs-lookup"><span data-stu-id="cbc79-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="cbc79-105">Về việc thực hiện thành công các PowerShell command(s), trang web gốc sẽ có một thông tin trang web trang chủ mới.</span><span class="sxs-lookup"><span data-stu-id="cbc79-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="cbc79-106">Thông tin chi tiết về các yêu cầu nào về tính năng và lệnh ghép ngắn PowerShell có sẵn trong bài viết [Cho phép-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="cbc79-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="cbc79-107">Chúng ta sẽ dần dần lăn ra, tắt theo mặc định, khách hàng nhắm mục tiêu phát hành đầu tháng năm 2019, và lăn ra sẽ có sẵn trên toàn thế giới bởi sự kết thúc của tháng 6 2019.</span><span class="sxs-lookup"><span data-stu-id="cbc79-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="cbc79-108">Tiếp tục đề cập đến [Thông báo Trung tâm](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) cho các tính năng mới khác với hiện đại.</span><span class="sxs-lookup"><span data-stu-id="cbc79-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="cbc79-109">**Chú ý**: không xóa trang web gốc cổ điển của bạn để tạo ra một trang web thông tin liên lạc hiện đại.</span><span class="sxs-lookup"><span data-stu-id="cbc79-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="cbc79-110">Điều này không được hỗ trợ bởi Microsoft.</span><span class="sxs-lookup"><span data-stu-id="cbc79-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="cbc79-111">Xóa trang web gốc sẽ làm cho tất cả các trang web SharePoint trong tổ chức của bạn không thể tiếp cận tất cả người dùng, cho đến khi bạn khôi phục lại các trang web hoặc tạo một trang web mới tại cùng một URL.</span><span class="sxs-lookup"><span data-stu-id="cbc79-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 