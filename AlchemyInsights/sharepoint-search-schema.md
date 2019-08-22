---
title: Quản lý các lược đồ tìm trong SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502829"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="27ff1-102">Quản lý các lược đồ tìm trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="27ff1-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="27ff1-103">Lược đồ tìm kiểm soát những gì người dùng có thể tìm kiếm, làm thế nào người dùng có thể tìm kiếm nó và làm thế nào bạn có thể trình bày các kết quả trên trang web tìm kiếm của bạn.</span><span class="sxs-lookup"><span data-stu-id="27ff1-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="27ff1-104">Hãy xem [quản lý giản đồ tìm trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) để tìm hiểu làm thế nào để:</span><span class="sxs-lookup"><span data-stu-id="27ff1-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="27ff1-105">Thay đổi lược đồ tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="27ff1-105">Change the search schema.</span></span>
- <span data-ttu-id="27ff1-106">Tạo quản lý tài sản.</span><span class="sxs-lookup"><span data-stu-id="27ff1-106">Create managed properties.</span></span>
- <span data-ttu-id="27ff1-107">Bản đồ thu thập thông tin bản đồ thu thập thông tin thuộc tính để quản lý tài sản.</span><span class="sxs-lookup"><span data-stu-id="27ff1-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="27ff1-108">Lưu ý sau đây liên quan đến việc quản lý lược đồ tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="27ff1-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="27ff1-109">Nếu bạn nhận được một cảnh báo nói rõ **ứng dụng bị tạm dừng** khi thực hiện một thay đổi lược đồ, điều này chỉ là tạm thời như là dịch vụ bảo trì xảy ra.</span><span class="sxs-lookup"><span data-stu-id="27ff1-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="27ff1-110">Nếu nhiều hơn 24 giờ đã trôi qua và bạn vẫn còn gặp các cảnh báo, xin vui lòng đăng nhập một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="27ff1-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="27ff1-111">Khi bạn thay đổi các thuộc tính được quản lý hoặc thêm những cái mới, những thay đổi có hiệu lực chỉ sau khi nội dung đã được tái crawled.</span><span class="sxs-lookup"><span data-stu-id="27ff1-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="27ff1-112">Trong SharePoint Online, thu thập dữ liệu xảy ra tự động dựa trên lịch trình thu thập dữ liệu được xác định.</span><span class="sxs-lookup"><span data-stu-id="27ff1-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="27ff1-113">Để đảm bảo rằng những thay đổi của bạn được thu thập thông tin, bạn có thể cụ thể [yêu cầu một tái lập chỉ mục các danh sách hoặc thư viện](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="27ff1-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="27ff1-114">Để hoàn thành nhìn của giản đồ tìm kiếm, hãy xem [Giới thiệu tìm Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="27ff1-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


