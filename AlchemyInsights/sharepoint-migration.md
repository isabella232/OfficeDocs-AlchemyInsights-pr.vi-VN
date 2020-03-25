---
title: Di chuyển các tùy chọn sang SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932752"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="f4968-102">Di chuyển các tùy chọn sang SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f4968-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="f4968-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="f4968-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f4968-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="f4968-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f4968-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="f4968-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f4968-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="f4968-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f4968-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="f4968-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f4968-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="f4968-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f4968-109">**Tùy chọn di chuyển**</span><span class="sxs-lookup"><span data-stu-id="f4968-109">**Migration options**</span></span>

<span data-ttu-id="f4968-110">Có các tùy chọn khác nhau có sẵn để di chuyển nội dung sang SharePoint Online, tùy thuộc vào kích thước và số lượng tệp bạn cần di chuyển, vui lòng xem danh sách các tùy chọn [nằm ở đây](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="f4968-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="f4968-111">Để biết thêm thông tin về di chuyển nội dung, vui lòng truy cập vào các liên kết bên dưới.</span><span class="sxs-lookup"><span data-stu-id="f4968-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="f4968-112">Công cụ di chuyển SharePoint</span><span class="sxs-lookup"><span data-stu-id="f4968-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="f4968-113">Bắt đầu với trình quản lý di chuyển</span><span class="sxs-lookup"><span data-stu-id="f4968-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="f4968-114">SharePoint Online và tốc độ di chuyển ODB</span><span class="sxs-lookup"><span data-stu-id="f4968-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="f4968-115">Tránh bị điều chỉnh hoặc chặn trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f4968-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="f4968-116">Công cụ đánh giá di chuyển SharePoint (SMAT)</span><span class="sxs-lookup"><span data-stu-id="f4968-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="f4968-117">**Lưu ý**: hiện tại công cụ SharePoint Migration chỉ hỗ trợ di chuyển từ SharePoint 2010 và 2013.</span><span class="sxs-lookup"><span data-stu-id="f4968-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="f4968-118">Phiên bản 2016 hoặc 2019 không được hỗ trợ tại thời gian này.</span><span class="sxs-lookup"><span data-stu-id="f4968-118">Version 2016 or 2019 are not supported at this time.</span></span>
