---
title: Điều chỉnh SharePoint trực tuyến
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931464"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="67f06-102">Điều chỉnh SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="67f06-102">SharePoint Online throttling</span></span>

<span data-ttu-id="67f06-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="67f06-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="67f06-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="67f06-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="67f06-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="67f06-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="67f06-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="67f06-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="67f06-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="67f06-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="67f06-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="67f06-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="67f06-109">**Điều chỉnh SharePoint trực tuyến**</span><span class="sxs-lookup"><span data-stu-id="67f06-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="67f06-110">SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch vụ SharePoint trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="67f06-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="67f06-111">Điều tiết giới hạn số hành động của người dùng hoặc các cuộc gọi đồng thời (theo tập lệnh hoặc mã) để tránh sử dụng quá nhiều tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="67f06-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="67f06-112">Để biết thêm thông tin, xin vui lòng truy cập vào các liên kết dưới đây.</span><span class="sxs-lookup"><span data-stu-id="67f06-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="67f06-113">Tránh bị điều chỉnh hoặc chặn trong SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="67f06-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="67f06-114">Di chuyển dữ liệu và điều chỉnh SPO</span><span class="sxs-lookup"><span data-stu-id="67f06-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="67f06-115">SharePoint Online và tốc độ di chuyển OneDrive</span><span class="sxs-lookup"><span data-stu-id="67f06-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="67f06-116">Xử lý SharePoint trực tuyến điều chỉnh bằng cách sử dụng mũ trở lại</span><span class="sxs-lookup"><span data-stu-id="67f06-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="67f06-117">Năng lực lập kế hoạch và tải thử nghiệm SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="67f06-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

