---
title: Hiệu suất di chuyển SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932410"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="63986-102">Hiệu suất di chuyển SharePoint</span><span class="sxs-lookup"><span data-stu-id="63986-102">SharePoint migration performance</span></span>

<span data-ttu-id="63986-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="63986-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="63986-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="63986-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="63986-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="63986-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="63986-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="63986-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="63986-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="63986-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="63986-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="63986-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="63986-109">**Hiệu suất di chuyển**</span><span class="sxs-lookup"><span data-stu-id="63986-109">**Migration performance**</span></span>

<span data-ttu-id="63986-110">Hiệu suất di chuyển có thể bị ảnh hưởng bởi cơ sở hạ tầng mạng, kích thước tệp, thời gian di chuyển và điều chỉnh.</span><span class="sxs-lookup"><span data-stu-id="63986-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="63986-111">Sự hiểu biết này sẽ giúp bạn lập kế hoạch và tối đa hóa hiệu quả di chuyển của bạn.</span><span class="sxs-lookup"><span data-stu-id="63986-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="63986-112">Để biết thêm thông tin, xin vui lòng truy cập vào các liên kết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="63986-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="63986-113">SharePoint Online và tốc độ di chuyển ODB</span><span class="sxs-lookup"><span data-stu-id="63986-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="63986-114">Tránh bị điều chỉnh hoặc chặn trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="63986-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="63986-115">Tải xuống và cài đặt công cụ di chuyển SharePoint</span><span class="sxs-lookup"><span data-stu-id="63986-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
