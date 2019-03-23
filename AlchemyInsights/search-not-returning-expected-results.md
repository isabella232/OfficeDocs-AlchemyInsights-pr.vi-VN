---
title: 1491-Search-not-Returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776103"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="54566-102">Tìm kiếm nội dung không phải trả lại kết quả mong đợi</span><span class="sxs-lookup"><span data-stu-id="54566-102">Content Search not returning expected results</span></span>

<span data-ttu-id="54566-103">Khi chạy nội dung tìm kiếm từ Office 365 an ninh & Trung tâm phù hợp, bạn có thể nhận được kết quả tìm kiếm không mong muốn.</span><span class="sxs-lookup"><span data-stu-id="54566-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="54566-104">Hãy xem xét những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="54566-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="54566-105">**Vị trí nội dung và các điều kiện tìm kiếm**: đảm bảo rằng bạn đã lựa chọn địa điểm thích hợp của nội dung và điều kiện tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="54566-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="54566-106">Nếu bạn chạy một tìm kiếm lớn (với nhiều địa điểm), xem xét việc chia tách nó thành nhiều tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="54566-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="54566-107">**Một phần được lập chỉ mục các mục**: [một phần được lập chỉ mục các mục](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) khỏi hộp thư được bao gồm trong kết quả tìm kiếm ước tính.</span><span class="sxs-lookup"><span data-stu-id="54566-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="54566-108">Tuy nhiên, các khoản mục được đánh chỉ mục một phần từ các trang web trong SharePoint và OneDrive không được bao gồm trong các ước tính tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="54566-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="54566-109">**Tìm kiếm thất bại**: khi tìm kiếm một số lượng lớn các hộp thư (hộp thư trên 100.000), bạn có thể nhận được lỗi tìm, với mã lỗi chẳng hạn như CS008-009 và CS012-002).</span><span class="sxs-lookup"><span data-stu-id="54566-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="54566-110">Trong trường hợp này, thử lại tìm kiếm chỉ cho các vị trí nội dung đã thất bại.</span><span class="sxs-lookup"><span data-stu-id="54566-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="54566-111">Xem [bài viết này](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="54566-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
