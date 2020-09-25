---
title: 1490-khắc phục sự cố-khám phá điện tử-hỏng
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277839"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="43243-102">Khắc phục lỗi tìm kiếm nội dung</span><span class="sxs-lookup"><span data-stu-id="43243-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="43243-103">Bạn gặp sự cố với tìm kiếm nội dung hoặc nhận được lỗi khi bạn xuất kết quả tìm kiếm?</span><span class="sxs-lookup"><span data-stu-id="43243-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="43243-104">Ví dụ, bạn có nhận được những thao tác sau khi tìm kiếm chạy không?</span><span class="sxs-lookup"><span data-stu-id="43243-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="43243-105">Lỗi CS008 hoặc CS012</span><span class="sxs-lookup"><span data-stu-id="43243-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="43243-106">Lỗi bận/thời gian chờ máy chủ</span><span class="sxs-lookup"><span data-stu-id="43243-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="43243-107">Lỗi ứng dụng đã xảy ra</span><span class="sxs-lookup"><span data-stu-id="43243-107">Application error occurred</span></span>

<span data-ttu-id="43243-108">Hoặc khi tìm kiếm hoặc xuất kết quả từ số lượng hộp thư lớn (trên hộp thư 100.000), thì bạn sẽ nhận được lỗi xuất hiện?</span><span class="sxs-lookup"><span data-stu-id="43243-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="43243-109">Đối với các loại lỗi này, hãy thử lại việc tìm kiếm các vị trí nội dung không thành công.</span><span class="sxs-lookup"><span data-stu-id="43243-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="43243-110">Xem  [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="43243-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="43243-111">Nếu bạn đang xuất nhiều hơn 100K hộp thư, bạn sẽ cần sử dụng PowerShell sau đây để tải xuống các kết quả xuất:  [xuất kết quả từ hơn 100k hộp thư](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="43243-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
