---
title: Tìm kiếm trong SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044065"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="259ea-102">Thu thập dữ liệu nội dung và lập chỉ mục trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="259ea-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="259ea-103">Nội dung phải được thu thập dữ liệu và thêm vào chỉ mục tìm kiếm để người dùng tìm thấy những gì họ đang tìm kiếm trong SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="259ea-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="259ea-104">Nội dung được tự động thu thập thông tin dựa trên lịch chạy dữ liệu được xác định trước (không thể thay đổi lịch thu thập dữ liệu).</span><span class="sxs-lookup"><span data-stu-id="259ea-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="259ea-105">Trình thu thập thông tin chọn lên nội dung đã thay đổi kể từ lần cuối và Cập Nhật chỉ mục.</span><span class="sxs-lookup"><span data-stu-id="259ea-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="259ea-106">Để đảm bảo nội dung được thu thập dữ liệu và chỉ mục được Cập Nhật, hãy lưu ý những mục sau:</span><span class="sxs-lookup"><span data-stu-id="259ea-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="259ea-107">Hãy chắc chắn rằng nội dung có thể được tìm thấy bằng cách [làm cho nội dung trang web tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="259ea-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="259ea-108">Khi bạn đã thay đổi thuộc tính được quản lý hoặc khi bạn đã thay đổi bản đồ của thuộc tính được quản lý và thu thập dữ liệu, trang web phải được tái thu thập dữ liệu trước khi thay đổi của bạn sẽ được phản ánh trong chỉ mục tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="259ea-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="259ea-109">Bởi vì các thay đổi của bạn được thực hiện trong sơ đồ tìm kiếm, và không phải là trang web thực tế, trình thu thập dữ liệu sẽ không tự động tái chỉ mục trang web.</span><span class="sxs-lookup"><span data-stu-id="259ea-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="259ea-110">Để biết thêm thông tin, xem [yêu cầu thu thập dữ liệu theo cách thủ công và lập chỉ mục lại một trang web, thư viện hoặc danh sách](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="259ea-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="259ea-111">Hãy đợi ít nhất 24 giờ sau khi yêu cầu chỉ mục thu thập dữ liệu và toàn bộ lại để xem bạn vẫn gặp sự cố hay chưa.</span><span class="sxs-lookup"><span data-stu-id="259ea-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="259ea-112">Nếu hơn 24 giờ đã trôi qua kể từ lúc bạn bắt đầu thu thập dữ liệu và chỉ mục lại đầy đủ, vui lòng đăng nhập một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="259ea-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="259ea-113">Trong nhiều trường hợp, chúng tôi đã làm việc trên một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="259ea-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="259ea-114">Xin vui lòng cho chúng tôi ít nhất 24 giờ để hoàn thành một giải pháp.</span><span class="sxs-lookup"><span data-stu-id="259ea-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="259ea-115">Nếu một trang web, tài liệu (thư viện) hoặc danh sách đã bị xoá và vẫn hiển thị trong kết quả tìm kiếm, người dùng sẽ nhận được **lỗi 404 tệp không tìm thấy** khi cố gắng truy cập.</span><span class="sxs-lookup"><span data-stu-id="259ea-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="259ea-116">Vấn đề này sẽ được đăng nhập như một trường hợp hỗ trợ để điều tra thêm.</span><span class="sxs-lookup"><span data-stu-id="259ea-116">This issue should be logged as a support case for further investigation.</span></span> 



