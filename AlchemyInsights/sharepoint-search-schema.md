---
title: Quản lý lược đồ tìm kiếm trong SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770573"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="84027-102">Quản lý lược đồ tìm kiếm trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="84027-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="84027-103">Lược đồ tìm kiếm điều khiển những người dùng có thể tìm kiếm, cách người dùng có thể tìm kiếm và cách bạn có thể trình bày kết quả trên các website tìm kiếm của mình.</span><span class="sxs-lookup"><span data-stu-id="84027-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="84027-104">Hãy xem [quản lý lược đồ tìm kiếm trong SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) để tìm hiểu cách:</span><span class="sxs-lookup"><span data-stu-id="84027-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="84027-105">Thay đổi lược đồ tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="84027-105">Change the search schema.</span></span>
- <span data-ttu-id="84027-106">Tạo thuộc tính được quản lý.</span><span class="sxs-lookup"><span data-stu-id="84027-106">Create managed properties.</span></span>
- <span data-ttu-id="84027-107">Bản đồ tìm kéo các thuộc tính được tìm kéo vào thuộc tính được quản lý.</span><span class="sxs-lookup"><span data-stu-id="84027-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="84027-108">Lưu ý những điều sau đây liên quan đến việc quản lý lược đồ tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="84027-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="84027-109">Nếu bạn nhận được một cảnh báo nêu rõ **ứng dụng sẽ bị tạm dừng** khi thực hiện thay đổi sơ đồ, điều này chỉ là tạm thời khi có bảo trì dịch vụ xảy ra.</span><span class="sxs-lookup"><span data-stu-id="84027-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="84027-110">Nếu có nhiều hơn 24 giờ đã trôi qua và bạn vẫn gặp phải cảnh báo, vui lòng đăng nhập một vụ việc hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="84027-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="84027-111">Khi bạn thay đổi các thuộc tính được quản lý hoặc thêm những thay đổi này chỉ có hiệu lực sau khi nội dung đã được thu thập lại.</span><span class="sxs-lookup"><span data-stu-id="84027-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="84027-112">Trong SharePoint Online, crawl sẽ xảy ra tự động dựa trên lịch trình thu thập được xác định.</span><span class="sxs-lookup"><span data-stu-id="84027-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="84027-113">Để đảm bảo rằng những thay đổi của bạn được thu thập, bạn có thể [yêu cầu một chỉ mục lại danh sách hoặc thư viện](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="84027-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="84027-114">Để biết tổng quan về sơ đồ tìm kiếm, hãy xem [giới thiệu lược đồ tìm kiếm](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="84027-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


