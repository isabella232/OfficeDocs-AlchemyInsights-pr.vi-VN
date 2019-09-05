---
title: Giới hạn SharePoint Online sang chế độ cổ điển
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752090"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="796c5-102">Giới hạn SharePoint Online sang chế độ cổ điển</span><span class="sxs-lookup"><span data-stu-id="796c5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="796c5-103">Một số tổ chức vẫn yêu cầu trải nghiệm chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="796c5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="796c5-104">Trong khi không có kế hoạch để loại bỏ chế độ cổ điển ở cấp độ chi tiết, nó không còn có thể hạn chế một tổ chức toàn bộ (người thuê nhà) để chế độ cổ điển cho các danh sách và thư viện.</span><span class="sxs-lookup"><span data-stu-id="796c5-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="796c5-105">Quản trị viên sẽ có các tùy chọn sau để quản lý các danh sách và thư viện riêng lẻ ở chế độ cổ điển sử dụng các công tắc chọn không tham gia chi tiết mà chúng tôi cung cấp ở các cấp sau:</span><span class="sxs-lookup"><span data-stu-id="796c5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="796c5-106">bộ sưu tập trang web</span><span class="sxs-lookup"><span data-stu-id="796c5-106">site collection</span></span>
- <span data-ttu-id="796c5-107">Trang web</span><span class="sxs-lookup"><span data-stu-id="796c5-107">site</span></span>
- <span data-ttu-id="796c5-108">Danh sách</span><span class="sxs-lookup"><span data-stu-id="796c5-108">list</span></span>
- <span data-ttu-id="796c5-109">Thư viện</span><span class="sxs-lookup"><span data-stu-id="796c5-109">library</span></span>

<span data-ttu-id="796c5-110">Ngoài ra, danh sách sử dụng một số tính năng và tuỳ chỉnh không được hỗ trợ bởi hiện đại sẽ vẫn được tự động chuyển sang chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="796c5-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="796c5-111">Bắt đầu từ ngày 1 tháng 4, 2019, quá trình này để vô hiệu hóa mức chọn không tham gia danh sách hiện đại và thư viện sẽ bắt đầu và tiếp tục thông qua ngày 31 tháng 5, 2019.</span><span class="sxs-lookup"><span data-stu-id="796c5-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="796c5-112">Các danh sách và thư viện ở chế độ cổ điển như là kết quả của việc chọn không tham gia thuê sẽ tự động được chuyển sang hiện đại.</span><span class="sxs-lookup"><span data-stu-id="796c5-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="796c5-113">Nếu bạn yêu cầu chế độ cổ điển xin vui lòng xem thêm thông tin [ở đây](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) và PNP PowerShell hướng dẫn [ở đây](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) mô tả các tùy chọn và công cụ bạn có thể sử dụng ngày hôm nay để sử dụng kinh nghiệm chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="796c5-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
