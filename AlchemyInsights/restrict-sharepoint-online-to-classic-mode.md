---
title: Giới hạn SharePoint Online với chế độ cổ điển
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751445"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="9a41e-102">Giới hạn SharePoint Online với chế độ cổ điển</span><span class="sxs-lookup"><span data-stu-id="9a41e-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="9a41e-103">Một số tổ chức vẫn yêu cầu trải nghiệm chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="9a41e-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="9a41e-104">Trong khi không có gói nào để loại bỏ chế độ cổ điển ở mức định dạng, nó không còn có thể hạn chế toàn bộ tổ chức (đối tượng thuê) đến chế độ cổ điển cho danh sách và thư viện.</span><span class="sxs-lookup"><span data-stu-id="9a41e-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="9a41e-105">Người quản trị sẽ có các tùy chọn sau đây để quản lý các danh sách và thư viện riêng lẻ trong chế độ cổ điển bằng cách chuyển đổi loại bỏ chọn tham gia mà chúng tôi cung cấp ở các cấp độ sau đây:</span><span class="sxs-lookup"><span data-stu-id="9a41e-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="9a41e-106">tuyển tập trang</span><span class="sxs-lookup"><span data-stu-id="9a41e-106">site collection</span></span>
- <span data-ttu-id="9a41e-107">đỗ</span><span class="sxs-lookup"><span data-stu-id="9a41e-107">site</span></span>
- <span data-ttu-id="9a41e-108">de</span><span class="sxs-lookup"><span data-stu-id="9a41e-108">list</span></span>
- <span data-ttu-id="9a41e-109">thư viện</span><span class="sxs-lookup"><span data-stu-id="9a41e-109">library</span></span>

<span data-ttu-id="9a41e-110">Ngoài ra, các danh sách sử dụng các tính năng và tùy chỉnh nhất định không được hiện đại hỗ trợ sẽ vẫn được tự động chuyển sang chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="9a41e-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="9a41e-111">Bắt đầu từ ngày 1 tháng 4, 2019, quy trình vô hiệu hóa mức đối tượng thuê không tham gia danh sách và thư viện hiện đại sẽ bắt đầu và tiếp tục đến ngày 31 tháng 5, 2019.</span><span class="sxs-lookup"><span data-stu-id="9a41e-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="9a41e-112">Các danh sách và thư viện trong chế độ cổ điển là kết quả của việc chọn không tham gia đối tượng thuê sẽ tự động được chuyển sang hiện đại.</span><span class="sxs-lookup"><span data-stu-id="9a41e-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="9a41e-113">Nếu bạn yêu cầu chế độ cổ điển vui lòng xem thêm thông tin [tại đây](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) và hướng dẫn về PNP PowerShell [ở đây](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) mô tả các tùy chọn và công cụ mà bạn có thể sử dụng hôm nay để sử dụng trải nghiệm chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="9a41e-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
