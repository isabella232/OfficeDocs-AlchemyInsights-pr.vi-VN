---
title: Quản lý sơ đồ tìm kiếm trong SharePoint trực tuyến
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042985"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="e3baf-102">Quản lý sơ đồ tìm kiếm trong SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="e3baf-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="e3baf-103">Sơ đồ tìm kiếm kiểm soát những gì người dùng có thể tìm kiếm, cách người dùng có thể tìm kiếm và cách bạn có thể trình bày kết quả trên các trang web tìm kiếm của mình.</span><span class="sxs-lookup"><span data-stu-id="e3baf-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="e3baf-104">Xem [quản lý sơ đồ tìm kiếm trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) để tìm hiểu cách:</span><span class="sxs-lookup"><span data-stu-id="e3baf-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="e3baf-105">Thay đổi sơ đồ tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="e3baf-105">Change the search schema.</span></span>
- <span data-ttu-id="e3baf-106">Tạo các tính được quản lý.</span><span class="sxs-lookup"><span data-stu-id="e3baf-106">Create managed properties.</span></span>
- <span data-ttu-id="e3baf-107">Bản đồ thu thập dữ liệu bản đồ cho các sản được quản lý.</span><span class="sxs-lookup"><span data-stu-id="e3baf-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="e3baf-108">Lưu ý như sau liên quan đến quản lý lược đồ tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="e3baf-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="e3baf-109">Nếu bạn nhận được một cảnh báo nói rằng **ứng dụng tạm dừng** khi thực hiện thay đổi sơ đồ, điều này chỉ là tạm thời là có dịch vụ bảo trì xảy ra.</span><span class="sxs-lookup"><span data-stu-id="e3baf-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="e3baf-110">Nếu hơn 24 giờ đã trôi qua và bạn vẫn gặp phải cảnh báo, vui lòng đăng nhập một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="e3baf-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="e3baf-111">Khi bạn thay đổi thuộc tính được quản lý hoặc thêm mới, các thay đổi có hiệu lực chỉ sau khi nội dung đã được thu thập lại.</span><span class="sxs-lookup"><span data-stu-id="e3baf-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="e3baf-112">Trong SharePoint trực tuyến, thu thập dữ liệu sẽ tự động dựa trên lịch trình crawl được xác định.</span><span class="sxs-lookup"><span data-stu-id="e3baf-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="e3baf-113">Để đảm bảo rằng các thay đổi của bạn được thu thập dữ liệu, bạn có thể [yêu cầu lập chỉ mục lại danh sách hoặc thư viện một cách](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) đặc biệt</span><span class="sxs-lookup"><span data-stu-id="e3baf-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="e3baf-114">Để biết tổng quan đầy đủ về sơ đồ tìm kiếm, hãy xem [giới thiệu sơ đồ tìm kiếm](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="e3baf-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


