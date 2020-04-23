---
title: SharePoint trực tuyến throttling
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 50b2c29db1fd294abe6c9e60f067156109de392b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742231"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="9cd2e-102">SharePoint trực tuyến throttling</span><span class="sxs-lookup"><span data-stu-id="9cd2e-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="9cd2e-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9cd2e-104">**503 Server là lỗi bận**</span><span class="sxs-lookup"><span data-stu-id="9cd2e-104">**503 server is busy error**</span></span>

<span data-ttu-id="9cd2e-105">Người dùng có thể nhận được một máy chủ 503 bận lỗi khi cố gắng di chuyển trang web SharePoint hoặc OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="9cd2e-106">Lỗi này có thể do điều chỉnh trong dịch vụ SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9cd2e-107">SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch vụ SharePoint trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9cd2e-108">Điều tiết giới hạn số hành động của người dùng hoặc các cuộc gọi đồng thời (theo tập lệnh hoặc mã) để tránh sử dụng quá nhiều tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="9cd2e-109">Để biết thêm thông tin về điều chỉnh xem, [tránh bị điều chỉnh hoặc chặn trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="9cd2e-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="9cd2e-110">Nếu bạn tin rằng lỗi này không liên quan đến điều chỉnh, bạn có thể kiểm tra nếu có bảo trì hoạt động xảy ra trên thuê của bạn bằng cách điều hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="9cd2e-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="9cd2e-111">Cuối cùng, đảm bảo bạn truy cập vào trang [y tế Dịch vụ](https://portal.office.com/adminportal/home#/servicehealth) để kiểm tra bất kỳ tư vấn/sự cố nào có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="9cd2e-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

