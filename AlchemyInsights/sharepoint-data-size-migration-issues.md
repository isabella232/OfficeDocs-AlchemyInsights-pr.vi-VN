---
title: Vấn đề trong khi di chuyển dữ liệu sang SharePoint trực tuyến
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931716"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="d1606-102">Vấn đề trong khi di chuyển dữ liệu sang SharePoint trực tuyến</span><span class="sxs-lookup"><span data-stu-id="d1606-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="d1606-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="d1606-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d1606-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="d1606-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d1606-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="d1606-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d1606-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="d1606-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d1606-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="d1606-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d1606-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="d1606-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d1606-109">**Di chuyển qua 100TB dữ liệu**</span><span class="sxs-lookup"><span data-stu-id="d1606-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="d1606-110">Nó xuất hiện bạn đang di chuyển qua 100TB dữ liệu sang SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d1606-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="d1606-111">Vui lòng làm theo các bước dưới đây để chúng tôi có thể hỗ trợ bạn sớm nhất có thể.</span><span class="sxs-lookup"><span data-stu-id="d1606-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="d1606-112">Chọn **yêu cầu dịch vụ mới**, và sau đó **yêu cầu dịch vụ mới**.</span><span class="sxs-lookup"><span data-stu-id="d1606-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="d1606-113">Để tiêu đề và mô tả là **di chuyển SharePoint qua 100TB**.</span><span class="sxs-lookup"><span data-stu-id="d1606-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="d1606-114">Sau khi đã gửi vé, vui lòng cập nhật thông tin sau:</span><span class="sxs-lookup"><span data-stu-id="d1606-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="d1606-115">Ước tính kích thước di chuyển của bạn.</span><span class="sxs-lookup"><span data-stu-id="d1606-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="d1606-116">Ước tính khi nào bạn muốn bắt đầu và hoàn tất di chuyển của mình.</span><span class="sxs-lookup"><span data-stu-id="d1606-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="d1606-117">Mô tả nơi bạn đang di chuyển nội dung của mình từ đó, chẳng hạn như SharePoint Server, Box, GDrive, chia sẻ tệp, v.v...</span><span class="sxs-lookup"><span data-stu-id="d1606-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

