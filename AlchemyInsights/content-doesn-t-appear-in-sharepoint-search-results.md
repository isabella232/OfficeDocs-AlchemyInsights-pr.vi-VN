---
title: Nội dung không xuất hiện trong kết quả tìm kiếm của SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363850"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="d83cd-102">Nội dung không xuất hiện trong kết quả tìm kiếm của SharePoint</span><span class="sxs-lookup"><span data-stu-id="d83cd-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="d83cd-103">Hãy làm theo các bước gỡ rối khi nội dung dự kiến sẽ không xuất hiện trong kết quả tìm kiếm:</span><span class="sxs-lookup"><span data-stu-id="d83cd-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="d83cd-104">Kiểm tra **trang web** có chứa nội dung dự kiến sẽ được thiết lập để cho phép nội dung xuất hiện trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="d83cd-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d83cd-105">Làm theo các bước trong [Hiển thị nội dung trên một trang web trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d83cd-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="d83cd-106">Kiểm tra **danh sách** hoặc **Thư viện** có chứa nội dung dự kiến sẽ được thiết lập để cho phép nội dung xuất hiện trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="d83cd-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="d83cd-107">Làm theo các bước trong [Hiển thị nội dung từ danh sách hoặc thư viện trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="d83cd-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="d83cd-108">Xác minh rằng trang, tài liệu hoặc trang tùy chỉnh bố trí được công bố như là một **lớn phiên bản.**</span><span class="sxs-lookup"><span data-stu-id="d83cd-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="d83cd-109">Thực hiện theo bước 3 trong [Tìm kiếm không trả lại tất cả kết quả trong SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="d83cd-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="d83cd-110">Xác minh rằng người dùng có **quyền** để xem nội dung.</span><span class="sxs-lookup"><span data-stu-id="d83cd-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="d83cd-111">Làm theo các bước trong [sự hiểu biết các cấp phép SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="d83cd-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="d83cd-112">Nếu lược đồ tìm kiếm đã được thay đổi bằng cách thêm một tài sản được quản lý mới, bằng cách chỉnh sửa một tài sản được quản lý, hoặc bằng cách loại bỏ một tài sản được quản lý, sau đó yêu cầu một thu thập dữ liệu và tái lập chỉ mục nhất sẽ được yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="d83cd-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="d83cd-113">**Lại chỉ mục** nội dung bằng cách làm theo các bước trong [tự yêu cầu thu thập dữ liệu và lập chỉ mục lại của một trang web, một thư viện hay một danh sách](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="d83cd-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="d83cd-114">Điều này có thể mất một lúc, hãy đợi 24 giờ trước khi kiểm tra kết quả một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="d83cd-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="d83cd-115">Để biết thêm chi tiết, hãy xem [sử nội dung trên một trang web để có thể tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="d83cd-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
