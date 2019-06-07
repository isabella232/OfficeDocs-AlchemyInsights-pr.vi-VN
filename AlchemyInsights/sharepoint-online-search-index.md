---
title: Quản lý các tìm kiếm từ điển trong SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758787"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="4c30e-102">Tìm kiếm trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4c30e-102">Search in SharePoint Online</span></span>

<span data-ttu-id="4c30e-103">Nội dung phải được thu thập và bổ sung vào danh mục tìm kiếm cho người dùng tìm thấy những gì họ đang tìm kiếm trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4c30e-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="4c30e-104">Nội dung được tự động thu thập thông tin dựa theo một lịch trình thu thập dữ liệu được xác định trước (lịch trình thu thập thông tin không thể được thay đổi).</span><span class="sxs-lookup"><span data-stu-id="4c30e-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="4c30e-105">Thu thập công cụ chọn lên nội dung đã thay đổi kể từ khi thu thập dữ liệu cuối cùng và Cập Nhật chỉ số.</span><span class="sxs-lookup"><span data-stu-id="4c30e-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="4c30e-106">Để đảm bảo nội dung thu thập thông tin và chỉ số được Cập Nhật, hãy làm theo các bước dưới đây.</span><span class="sxs-lookup"><span data-stu-id="4c30e-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="4c30e-107">Đảm bảo rằng nội dung có thể được tìm thấy bằng cách tìm kiếm nội dung trang web.</span><span class="sxs-lookup"><span data-stu-id="4c30e-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="4c30e-108">Để biết thêm chi tiết, hãy xem [sử nội dung trên một trang web để có thể tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="4c30e-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="4c30e-109">Khi bạn đã thay đổi một tài sản được quản lý, hoặc khi bạn đã thay đổi bản đồ của thu thập và quản lý tài sản, các trang web phải được tái crawled trước khi thay đổi của bạn sẽ được phản ánh trong chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="4c30e-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="4c30e-110">Bởi vì các thay đổi được thực hiện trong lược đồ tìm kiếm, và không để các trang web thực tế, các trình thu thập sẽ không tự động tái index trang web.</span><span class="sxs-lookup"><span data-stu-id="4c30e-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="4c30e-111">Để biết thêm chi tiết, hãy xem [theo cách thủ công yêu cầu thu thập dữ liệu và lập chỉ mục lại của một trang web, một thư viện hay một danh sách](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="4c30e-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="4c30e-112">Đợi ít nhất 24 giờ sau khi theo cách thủ công yêu cầu một thu thập thông tin và đầy đủ tái lập chỉ mục để xem nếu bạn vẫn gặp sự cố.</span><span class="sxs-lookup"><span data-stu-id="4c30e-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="4c30e-113">Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn bắt đầu thu thập dữ liệu và lập chỉ mục lại đầy đủ, xin vui lòng đăng nhập một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="4c30e-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="4c30e-114">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="4c30e-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4c30e-115">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="4c30e-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="4c30e-116">**Chú ý**: nếu một trang web, tài liệu (thư viện), hoặc một danh sách đã bị xoá và vẫn thấy trong kết quả tìm kiếm, người dùng sẽ nhận được một lỗi 404 Không tìm thấy tệp khi cố gắng truy cập.</span><span class="sxs-lookup"><span data-stu-id="4c30e-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="4c30e-117">Vấn đề này nên được đăng nhập như là một trường hợp hỗ trợ cho điều tra thêm.</span><span class="sxs-lookup"><span data-stu-id="4c30e-117">This issue should be logged as a support case for further investigation.</span></span> 



