---
title: 1491-tìm kiếm-không-trở lại-dự kiến-kết quả
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709249"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="004bc-102">Tìm kiếm nội dung không trả lại kết quả mong đợi</span><span class="sxs-lookup"><span data-stu-id="004bc-102">Content Search not returning expected results</span></span>

<span data-ttu-id="004bc-103">Khi chạy tìm kiếm nội dung từ Microsoft 365 bảo mật & Trung tâm tuân thủ, bạn có thể nhận được kết quả tìm kiếm không mong muốn.</span><span class="sxs-lookup"><span data-stu-id="004bc-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="004bc-104">Hãy xem xét những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="004bc-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="004bc-105">**Vị trí nội dung và điều kiện tìm kiếm**: đảm bảo bạn đã chọn vị trí nội dung phù hợp và điều kiện tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="004bc-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="004bc-106">Nếu bạn chạy một tìm kiếm lớn (với nhiều vị trí), hãy xem xét chia tách nó thành nhiều tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="004bc-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="004bc-107">**Mục đã lập chỉ mục một**phần: các [mục đã lập chỉ mục một phần](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) từ hộp thư được bao gồm trong kết quả tìm kiếm ước tính.</span><span class="sxs-lookup"><span data-stu-id="004bc-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="004bc-108">Tuy nhiên, một phần được lập chỉ mục từ các trang web trong SharePoint và OneDrive không được bao gồm trong ước tính tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="004bc-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="004bc-109">Lỗi **Tìm kiếm**: khi tìm kiếm một số lượng lớn hộp thư (trên 100.000 hộp thư), bạn có thể nhận được lỗi tìm kiếm, với mã lỗi như CS008-009 và CS012-002).</span><span class="sxs-lookup"><span data-stu-id="004bc-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="004bc-110">Trong trường hợp này, thử tìm kiếm chỉ cho các vị trí nội dung không thành công.</span><span class="sxs-lookup"><span data-stu-id="004bc-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="004bc-111">Xem [bài viết này](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="004bc-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
