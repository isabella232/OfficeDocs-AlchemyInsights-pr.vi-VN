---
title: 1491-tìm kiếm-không-trả về-kết quả dự kiến
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740496"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="ace0a-102">Tìm kiếm nội dung không trả về kết quả dự kiến</span><span class="sxs-lookup"><span data-stu-id="ace0a-102">Content Search not returning expected results</span></span>

<span data-ttu-id="ace0a-103">Khi chạy các tìm kiếm nội dung từ Trung tâm tuân thủ & bảo mật của Microsoft 365, bạn có thể nhận được kết quả tìm kiếm không mong muốn.</span><span class="sxs-lookup"><span data-stu-id="ace0a-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="ace0a-104">Hãy cân nhắc những điều sau đây có thể ảnh hưởng đến kết quả tìm kiếm của bạn:</span><span class="sxs-lookup"><span data-stu-id="ace0a-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="ace0a-105">**Vị trí nội dung và điều kiện tìm kiếm**: đảm bảo rằng bạn đã chọn các vị trí nội dung thích hợp và các điều kiện tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="ace0a-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="ace0a-106">Nếu bạn đã chạy tìm kiếm lớn (với nhiều vị trí), hãy cân nhắc chia tách nó thành nhiều tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="ace0a-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="ace0a-107">Các **mục được lập chỉ mục một phần**: các [mục được lập chỉ mục một phần](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) từ hộp thư được bao gồm trong kết quả tìm kiếm ước tính.</span><span class="sxs-lookup"><span data-stu-id="ace0a-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="ace0a-108">Tuy nhiên, các mục được lập chỉ mục một phần từ các site trong SharePoint và OneDrive không được bao gồm trong ước tính tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="ace0a-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="ace0a-109">Lỗi **Tìm kiếm**: khi tìm kiếm số lượng hộp thư lớn (trên hộp thư 100.000), bạn có thể gặp lỗi tìm kiếm, với các mã lỗi chẳng hạn như CS008-009 và CS012-002).</span><span class="sxs-lookup"><span data-stu-id="ace0a-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="ace0a-110">Trong trường hợp này, hãy thử lại chỉ tìm kiếm cho các vị trí nội dung không thành công.</span><span class="sxs-lookup"><span data-stu-id="ace0a-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="ace0a-111">Xem  [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="ace0a-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
