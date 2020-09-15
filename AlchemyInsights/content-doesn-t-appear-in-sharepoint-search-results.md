---
title: Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713152"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="a1004-102">Nội dung không xuất hiện trong kết quả tìm kiếm SharePoint</span><span class="sxs-lookup"><span data-stu-id="a1004-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="a1004-103">Hãy làm theo các bước khắc phục sự cố này khi nội dung được dự kiến không xuất hiện trong kết quả tìm kiếm:</span><span class="sxs-lookup"><span data-stu-id="a1004-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="a1004-104">Kiểm tra xem **trang** có chứa nội dung được dự kiến được đặt là cho phép nội dung xuất hiện trong kết quả tìm kiếm hay không.</span><span class="sxs-lookup"><span data-stu-id="a1004-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="a1004-105">Làm theo các bước trong [Hiển thị nội dung trên một trang trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="a1004-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="a1004-106">Kiểm tra xem **danh sách** hoặc **Thư viện** có chứa nội dung được dự kiến được đặt là cho phép nội dung xuất hiện trong kết quả tìm kiếm hay không.</span><span class="sxs-lookup"><span data-stu-id="a1004-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="a1004-107">Làm theo các bước trong [Hiển thị nội dung từ danh sách hoặc thư viện trong kết quả tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="a1004-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="a1004-108">Xác minh rằng trang, tài liệu hoặc bố trí trang tùy chỉnh được phát hành dưới dạng **Phiên bản chính.**</span><span class="sxs-lookup"><span data-stu-id="a1004-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="a1004-109">Làm theo bước 3 trong [Tìm kiếm không trả về tất cả các kết quả trong SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="a1004-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="a1004-110">Xác nhận rằng người dùng có **quyền** xem nội dung.</span><span class="sxs-lookup"><span data-stu-id="a1004-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="a1004-111">Làm theo các bước trong [Tìm hiểu các mức cấp phép trong SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="a1004-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="a1004-112">Nếu sơ đồ tìm kiếm đã được thay đổi bằng cách thêm một thuộc tính được quản lý mới, bằng cách sửa thuộc tính được quản lý hoặc loại bỏ một thuộc tính được quản lý sau đó yêu cầu thu thập và chỉ mục lại sẽ được yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="a1004-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="a1004-113">Lập **chỉ mục lại** nội dung bằng cách thực hiện theo các bước bằng cách thủ công theo [yêu cầu thu thập và lập chỉ mục lại một site, một thư viện hoặc danh sách](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="a1004-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="a1004-114">Việc này có thể mất một lúc, chờ 24 giờ trước khi kiểm tra lại kết quả.</span><span class="sxs-lookup"><span data-stu-id="a1004-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="a1004-115">Để biết thêm thông tin, hãy xem mục [bật nội dung trên một trang để có thể tìm kiếm](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="a1004-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
