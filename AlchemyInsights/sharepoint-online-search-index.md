---
title: Tìm kiếm trong SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507653"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="1612b-102">Nội dung thu thập dữ liệu và lập chỉ mục trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="1612b-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="1612b-103">Nội dung phải được thu thập và bổ sung vào danh mục tìm kiếm cho người dùng tìm thấy những gì họ đang tìm kiếm trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1612b-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="1612b-104">Nội dung được tự động thu thập thông tin dựa theo một lịch trình thu thập dữ liệu được xác định trước (lịch trình thu thập thông tin không thể được thay đổi).</span><span class="sxs-lookup"><span data-stu-id="1612b-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="1612b-105">Thu thập công cụ chọn lên nội dung đã thay đổi kể từ khi thu thập dữ liệu cuối cùng và Cập Nhật chỉ số.</span><span class="sxs-lookup"><span data-stu-id="1612b-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="1612b-106">Để đảm bảo nội dung thu thập thông tin và chỉ số được Cập Nhật, lưu ý những điều sau đây:</span><span class="sxs-lookup"><span data-stu-id="1612b-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="1612b-107">Đảm bảo rằng nội dung có thể được tìm thấy bằng [cách tìm kiếm nội dung trang web](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="1612b-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="1612b-108">Khi bạn đã thay đổi một tài sản được quản lý, hoặc khi bạn đã thay đổi bản đồ của thu thập và quản lý tài sản, các trang web phải được tái crawled trước khi thay đổi của bạn sẽ được phản ánh trong chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="1612b-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="1612b-109">Bởi vì các thay đổi được thực hiện trong lược đồ tìm kiếm, và không để các trang web thực tế, các trình thu thập sẽ không tự động tái index trang web.</span><span class="sxs-lookup"><span data-stu-id="1612b-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="1612b-110">Để biết thêm chi tiết, hãy xem [theo cách thủ công yêu cầu thu thập dữ liệu và lập chỉ mục lại của một trang web, một thư viện hay một danh sách](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="1612b-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="1612b-111">Đợi ít nhất 24 giờ sau khi theo cách thủ công yêu cầu một thu thập thông tin và đầy đủ tái lập chỉ mục để xem nếu bạn vẫn gặp sự cố.</span><span class="sxs-lookup"><span data-stu-id="1612b-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="1612b-112">Nếu nhiều hơn 24 giờ đã trôi qua kể từ khi bạn bắt đầu thu thập dữ liệu và lập chỉ mục lại đầy đủ, xin vui lòng đăng nhập một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="1612b-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="1612b-113">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="1612b-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1612b-114">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="1612b-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1612b-115">Nếu một trang web, tài liệu (thư viện), hoặc một danh sách đã bị xoá và vẫn cho thấy trong kết quả tìm kiếm, người dùng sẽ nhận được một **Lỗi 404 Không tìm thấy tệp** khi cố gắng để truy cập vào nó.</span><span class="sxs-lookup"><span data-stu-id="1612b-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="1612b-116">Vấn đề này nên được đăng nhập như là một trường hợp hỗ trợ cho điều tra thêm.</span><span class="sxs-lookup"><span data-stu-id="1612b-116">This issue should be logged as a support case for further investigation.</span></span> 



