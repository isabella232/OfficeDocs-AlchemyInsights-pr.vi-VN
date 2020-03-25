---
title: SharePoint di chuyển điều chỉnh với 503 lỗi
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931680"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="19f37-102">SharePoint di chuyển điều chỉnh với 503 lỗi</span><span class="sxs-lookup"><span data-stu-id="19f37-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="19f37-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="19f37-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="19f37-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="19f37-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="19f37-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="19f37-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="19f37-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="19f37-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="19f37-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="19f37-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="19f37-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="19f37-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="19f37-109">**503 lỗi khi di chuyển sang SharePoint trực tuyến**</span><span class="sxs-lookup"><span data-stu-id="19f37-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="19f37-110">Nó xuất hiện bạn đang di chuyển sang SharePoint trực tuyến và nhận được lỗi 503.</span><span class="sxs-lookup"><span data-stu-id="19f37-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="19f37-111">Vui lòng làm theo các bước dưới đây để chúng tôi có thể hỗ trợ bạn sớm nhất có thể.</span><span class="sxs-lookup"><span data-stu-id="19f37-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="19f37-112">Bấm vào **hỗ trợ liên hệ**, và sau đó **yêu cầu dịch vụ mới**.</span><span class="sxs-lookup"><span data-stu-id="19f37-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="19f37-113">Tiêu đề và mô tả, nhập **SharePoint Migration throttling với 503**.</span><span class="sxs-lookup"><span data-stu-id="19f37-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="19f37-114">Sau khi đã gửi vé, vui lòng cập nhật thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="19f37-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="19f37-115">Bao nhiêu trái của di cư (ví dụ, bao nhiêu TBs?).</span><span class="sxs-lookup"><span data-stu-id="19f37-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="19f37-116">Ngày bắt đầu và kết thúc di chuyển.</span><span class="sxs-lookup"><span data-stu-id="19f37-116">Migration start and end date.</span></span>
    - <span data-ttu-id="19f37-117">Mô tả nơi bạn đang di chuyển nội dung của mình từ đó, chẳng hạn như SharePoint Server, Box, GDrive, chia sẻ tệp, v.v...</span><span class="sxs-lookup"><span data-stu-id="19f37-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="19f37-118">Ước tính số điều chỉnh lỗi (ví dụ: x throttle mỗi giờ?) và khi điều chỉnh xảy ra.</span><span class="sxs-lookup"><span data-stu-id="19f37-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="19f37-119">Bạn đang sử dụng công cụ di chuyển nào (ví dụ: SPMT hoặc ShareGate).</span><span class="sxs-lookup"><span data-stu-id="19f37-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


