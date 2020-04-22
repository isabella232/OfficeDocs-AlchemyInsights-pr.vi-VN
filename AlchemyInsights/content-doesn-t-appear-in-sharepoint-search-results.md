---
title: Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705683"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="092c8-102">Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint</span><span class="sxs-lookup"><span data-stu-id="092c8-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="092c8-103">Thực hiện theo các bước khắc phục sự cố khi mong muốn nội dung không xuất hiện trong kết quả tìm kiếm:</span><span class="sxs-lookup"><span data-stu-id="092c8-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="092c8-104">Kiểm tra xem **trang web** chứa nội dung mong muốn được đặt để cho phép nội dung xuất hiện trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="092c8-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="092c8-105">Làm theo các bước trong [Hiển thị nội dung trên một trang web trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="092c8-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="092c8-106">Kiểm tra xem **danh sách** hoặc **Thư viện** có chứa nội dung mong muốn được đặt để cho phép nội dung xuất hiện trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="092c8-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="092c8-107">Làm theo các bước trong [Hiển thị nội dung từ danh sách hoặc thư viện trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="092c8-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="092c8-108">Xác minh rằng trang, tài liệu hoặc bố cục trang tùy chỉnh được xuất bản dưới dạng một **Phiên bản chính.**</span><span class="sxs-lookup"><span data-stu-id="092c8-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="092c8-109">Làm theo bước 3 trong [Tìm kiếm không trả lại tất cả các kết quả trong SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="092c8-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="092c8-110">Xác minh rằng người dùng có **quyền** để xem nội dung.</span><span class="sxs-lookup"><span data-stu-id="092c8-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="092c8-111">Làm theo các bước trong [hiểu biết cấp quyền trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="092c8-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="092c8-112">Nếu sơ đồ tìm kiếm đã được thay đổi bằng cách thêm một thuộc tính được quản lý mới, bằng cách chỉnh sửa một thuộc tính được quản lý, hoặc bằng cách loại bỏ một thuộc tính quản lý sau đó yêu cầu thu thập dữ liệu và tái chỉ mục sẽ được yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="092c8-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="092c8-113">**Tái chỉ mục** nội dung bằng cách làm theo các bước trong [thủ công yêu cầu thu thập và lập chỉ mục lại một trang web, một thư viện hoặc một danh sách](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="092c8-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="092c8-114">Điều này có thể mất một lúc, đợi 24 giờ trước khi kiểm tra kết quả một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="092c8-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="092c8-115">Để biết thêm thông tin, hãy xem cho [phép tìm kiếm nội dung trên trang web](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="092c8-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
