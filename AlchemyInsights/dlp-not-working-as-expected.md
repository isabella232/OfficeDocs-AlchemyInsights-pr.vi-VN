---
title: DLP không làm việc như mong đợi
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0d50ac1aed1bd8168daa45e33b6e0bc37e95d1b7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661995"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="8e18d-102">DLP không làm việc như mong đợi</span><span class="sxs-lookup"><span data-stu-id="8e18d-102">DLP not working as expected</span></span>


<span data-ttu-id="8e18d-p101">Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** trong Office 365 không làm việc như mong đợi? Nếu vậy, hãy chắc chắn rằng bạn **chính sách DLP** là thiết lập một cách chính xác, và dữ liệu của bạn có chứa những gì **chính sách DLP** tìm kiếm khi nó đang được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="8e18d-p101">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected? If so, make sure that your **DLP policy** is setup correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="8e18d-105">**Thiết lập DLP:**</span><span class="sxs-lookup"><span data-stu-id="8e18d-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="8e18d-p102">DLP chính sách cho phép bạn xác định và bảo vệ các thông tin nhạy cảm trong tổ chức của bạn. Để thiết lập chính sách DLP, sử dụng các thông tin [ở đây](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="8e18d-p102">DLP policies allows you to identify and protect sensitive information in your organization. To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="8e18d-108">**Những gì chính sách DLP tìm:**</span><span class="sxs-lookup"><span data-stu-id="8e18d-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="8e18d-109">Khi sử dụng **các loại thông tin nhạy cảm được xây dựng trong** Trung tâm văn phòng 365 bảo mật và tuân thủ, DLP chính sách tìm mô hình cụ thể và các yếu tố khi phát hiện những loại nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="8e18d-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="8e18d-110">**Thông tin nhạy cảm được xây dựng trong các loại:**</span><span class="sxs-lookup"><span data-stu-id="8e18d-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="8e18d-111">Thông tin về các loại nhạy cảm được xây dựng trong và những gì một chính sách DLP trông khi phát hiện các loại nhạy cảm, nhìn thấy: [những thông tin nhạy cảm loại tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="8e18d-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="8e18d-112">**Các loại thông tin nhạy cảm tùy chỉnh:**</span><span class="sxs-lookup"><span data-stu-id="8e18d-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="8e18d-113">Nếu bạn đang cố gắng để tạo ra các loại tùy chỉnh các thông tin nhạy cảm, sử dụng bài viết sau để biết thông tin về làm thế nào để tạo ra một loại nhạy cảm tùy chỉnh: [tạo một loại tùy chỉnh các thông tin nhạy cảm](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8e18d-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="8e18d-114">**Báo cáo:**</span><span class="sxs-lookup"><span data-stu-id="8e18d-114">**Reports:**</span></span>
  
- <span data-ttu-id="8e18d-115">Nhận được dữ liệu nhạy cảm hiểu biết với [báo cáo DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="8e18d-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="8e18d-116">Xem thông tin chi tiết cụ thể của sự kiện với một [Báo cáo Incident](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="8e18d-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

