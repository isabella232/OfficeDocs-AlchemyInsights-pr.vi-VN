---
title: Sử versioning trong một danh sách hoặc thư viện
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.openlocfilehash: d75ce74f32e4d51fa18e49a853c7a6a3da641240
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223626"
---
# <a name="enable-versioning-for-a-sharepoint-list-or-library"></a><span data-ttu-id="c13b0-102">Sử versioning cho một danh sách SharePoint hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="c13b0-102">Enable versioning for a SharePoint list or library</span></span>


<span data-ttu-id="c13b0-103">Khi versioning được kích hoạt trong danh sách SharePoint hoặc thư viện của bạn, bạn có thể lưu trữ, theo dõi và khôi phục các khoản mục trong danh sách và các tập tin trong một thư viện bất cứ khi nào họ thay đổi.</span><span class="sxs-lookup"><span data-stu-id="c13b0-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="c13b0-104">Versioning, kết hợp với các cài đặt khác, chẳng hạn như thanh toán, cung cấp cho bạn nhiều quyền kiểm soát nội dung được đăng trên trang web của bạn và có thể cung cấp giá trị thực sự nếu bạn đã bao giờ có một nhu cầu để xem hoặc khôi phục lại phiên bản cũ của một mục hoặc tập tin.</span><span class="sxs-lookup"><span data-stu-id="c13b0-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="c13b0-105">Để biết thêm thông tin về versioning xin vui lòng truy cập vào các bên dưới bài viết.</span><span class="sxs-lookup"><span data-stu-id="c13b0-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="c13b0-106">Versioning thế nào trong danh sách SharePoint hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="c13b0-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="c13b0-107">Kích hoạt và đặt cấu hình versioning cho một danh sách hoặc thư viện</span><span class="sxs-lookup"><span data-stu-id="c13b0-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f&amp;ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="c13b0-108">Làm thế nào để xem lịch sử Phiên bản</span><span class="sxs-lookup"><span data-stu-id="c13b0-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="c13b0-109">Khôi phục Phiên bản trước của một tập tin trong OneDrive</span><span class="sxs-lookup"><span data-stu-id="c13b0-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893?ui=en-US&amp;rs=en-US&amp;ad=US)

- [<span data-ttu-id="c13b0-110">Xem các phiên bản trước đó của tệp Office</span><span class="sxs-lookup"><span data-stu-id="c13b0-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="c13b0-111">Giới hạn versioning</span><span class="sxs-lookup"><span data-stu-id="c13b0-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

<span data-ttu-id="c13b0-112">**Lưu ý:** Nếu bạn là một khách hàng Office 365, versioning được bây giờ bật theo mặc định khi bạn tạo mới OneDrive cho doanh nghiệp thư viện, và nó sẽ tự động lưu qua 500 các phiên bản của một tài liệu.</span><span class="sxs-lookup"><span data-stu-id="c13b0-112">**Note:** If you are an Office 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="c13b0-113">Điều này sẽ giúp bạn ngăn ngừa mất dữ liệu hoặc tài liệu quan trọng.</span><span class="sxs-lookup"><span data-stu-id="c13b0-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="c13b0-114">Nếu bạn có các thư viện hiện có vào OneDrive của bạn cho trang web kinh doanh, hoặc trên trang web đội ngũ của bạn mà không cần versioning được kích hoạt, bạn có thể bật versioning cho họ bất cứ lúc nào.</span><span class="sxs-lookup"><span data-stu-id="c13b0-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


