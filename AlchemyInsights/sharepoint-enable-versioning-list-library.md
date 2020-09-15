---
title: Lập phiên bản trong SharePoint và OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 12207efc9822be6cf096fa4884a3cd244a286cbe
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653751"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="c1679-102">Lập phiên bản trong SharePoint và OneDrive</span><span class="sxs-lookup"><span data-stu-id="c1679-102">Versioning in SharePoint and OneDrive</span></span> 


<span data-ttu-id="c1679-103">Khi lập phiên bản được bật trong danh sách hoặc thư viện SharePoint của bạn, bạn có thể lưu trữ, theo dõi và khôi phục các mục trong danh sách và tệp trong thư viện bất cứ khi nào thay đổi.</span><span class="sxs-lookup"><span data-stu-id="c1679-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="c1679-104">Lập phiên bản, kết hợp với các thiết đặt khác, chẳng hạn như Checkout, cung cấp cho bạn nhiều quyền kiểm soát nội dung được đăng trên trang web của bạn và có thể cung cấp giá trị thực nếu bạn đã bao giờ cần phải xem hoặc khôi phục Phiên bản cũ của một mục hoặc tệp.</span><span class="sxs-lookup"><span data-stu-id="c1679-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="c1679-105">Để biết thêm thông tin về lập phiên bản xin vui lòng truy cập các bài viết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="c1679-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="c1679-106">Lập phiên bản hoạt động như thế nào trong danh sách hoặc thư viện SharePoint</span><span class="sxs-lookup"><span data-stu-id="c1679-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="c1679-107">Bật và cấu hình lập phiên bản cho một danh sách hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="c1679-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f)

- [<span data-ttu-id="c1679-108">Cách xem lịch sử Phiên bản</span><span class="sxs-lookup"><span data-stu-id="c1679-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="c1679-109">Khôi phục Phiên bản trước của tệp trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="c1679-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893)

- [<span data-ttu-id="c1679-110">Xem các phiên bản trước đó của tệp Office</span><span class="sxs-lookup"><span data-stu-id="c1679-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="c1679-111">Giới hạn lập phiên bản</span><span class="sxs-lookup"><span data-stu-id="c1679-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="c1679-112">Nếu bạn là khách hàng của Microsoft 365, phiên bản hiện tại được bật theo mặc định khi bạn tạo thư viện OneDrive for Business mới, và nó sẽ tự động lưu các phiên bản 500 cuối cùng của tài liệu.</span><span class="sxs-lookup"><span data-stu-id="c1679-112">If you are a Microsoft 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="c1679-113">Điều này sẽ giúp bạn ngăn không cho mất tài liệu hoặc dữ liệu quan trọng.</span><span class="sxs-lookup"><span data-stu-id="c1679-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="c1679-114">Nếu bạn có các thư viện hiện có trên site OneDrive for Business của mình hoặc trên site nhóm của mình, bạn có thể bật tính năng lập phiên bản cho họ bất kỳ lúc nào.</span><span class="sxs-lookup"><span data-stu-id="c1679-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


