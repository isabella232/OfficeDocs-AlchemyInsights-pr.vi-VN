---
title: SharePoint trực tuyến throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931248"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="3aa92-102">SharePoint trực tuyến throttling</span><span class="sxs-lookup"><span data-stu-id="3aa92-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="3aa92-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="3aa92-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="3aa92-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="3aa92-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="3aa92-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="3aa92-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="3aa92-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="3aa92-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="3aa92-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="3aa92-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="3aa92-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="3aa92-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="3aa92-109">**503 Server là lỗi bận**</span><span class="sxs-lookup"><span data-stu-id="3aa92-109">**503 server is busy error**</span></span>

<span data-ttu-id="3aa92-110">Người dùng có thể nhận được một máy chủ 503 bận lỗi khi cố gắng di chuyển trang web SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3aa92-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="3aa92-111">Lỗi này có thể do điều chỉnh trong dịch vụ SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3aa92-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="3aa92-112">SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch vụ SharePoint trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="3aa92-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="3aa92-113">Điều tiết giới hạn số hành động của người dùng hoặc các cuộc gọi đồng thời (theo tập lệnh hoặc mã) để tránh sử dụng quá nhiều tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="3aa92-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="3aa92-114">Để biết thêm thông tin về điều chỉnh xem, [tránh bị điều chỉnh hoặc chặn trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="3aa92-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="3aa92-115">Nếu bạn tin rằng lỗi này không liên quan đến điều chỉnh, bạn có thể kiểm tra nếu có bảo trì hoạt động xảy ra trên thuê của bạn bằng cách điều hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="3aa92-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="3aa92-116">Cuối cùng, đảm bảo bạn truy cập vào trang [y tế Dịch vụ](https://portal.office.com/adminportal/home#/servicehealth) để kiểm tra bất kỳ tư vấn/sự cố nào có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="3aa92-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

