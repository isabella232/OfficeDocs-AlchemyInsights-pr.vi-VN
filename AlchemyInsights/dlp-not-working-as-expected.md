---
title: DLP không hoạt động như mong đợi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507500"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="e2b06-102">DLP không hoạt động như mong đợi</span><span class="sxs-lookup"><span data-stu-id="e2b06-102">DLP not working as expected</span></span>

<span data-ttu-id="e2b06-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="e2b06-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="e2b06-104">**Thiết lập DLP**</span><span class="sxs-lookup"><span data-stu-id="e2b06-104">**Setting up DLP**</span></span>

<span data-ttu-id="e2b06-105">Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** trong Office 365 không hoạt động như mong đợi?</span><span class="sxs-lookup"><span data-stu-id="e2b06-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="e2b06-106">Nếu có, đảm bảo rằng **chính sách DLP** của bạn được thiết lập chính xác và dữ liệu của bạn chứa những gì **chính sách DLP** đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="e2b06-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="e2b06-107">Chính sách DLP cho phép bạn xác định và bảo vệ thông tin nhạy cảm trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="e2b06-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="e2b06-108">Thiết lập chính sách DLP, sử dụng thông tin [ở đây](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="e2b06-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="e2b06-109">**Chính sách DLP nào tìm kiếm**</span><span class="sxs-lookup"><span data-stu-id="e2b06-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="e2b06-110">Khi sử dụng các **loại thông tin nhạy cảm tích hợp** trong Trung tâm bảo mật và tuân thủ, chính sách DLP tìm các mẫu và yếu tố cụ thể khi phát hiện các loại nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="e2b06-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="e2b06-111">**Tích hợp các loại thông tin nhạy cảm**</span><span class="sxs-lookup"><span data-stu-id="e2b06-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="e2b06-112">Để biết thông tin về các loại nhạy cảm và chính sách DLP sẽ tìm kiếm khi phát hiện loại nhạy cảm, hãy xem: [những loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="e2b06-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="e2b06-113">**Các loại thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="e2b06-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="e2b06-114">Nếu bạn đang cố gắng tạo các loại thông tin nhạy cảm tùy chỉnh, hãy sử dụng bài viết sau để biết thông tin về cách tạo loại nhạy cảm tùy chỉnh: [tạo loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="e2b06-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="e2b06-115">**Kiểm tra chính sách DLP**</span><span class="sxs-lookup"><span data-stu-id="e2b06-115">**Test a DLP policy**</span></span>

<span data-ttu-id="e2b06-116">Để kiểm tra dữ liệu của bạn bằng loại thông tin nhạy cảm được tích hợp hoặc tùy chỉnh, hãy sử dụng tùy chọn **loại thử nghiệm** **trong phân**  >  **loại thông tin nhạy cảm**.</span><span class="sxs-lookup"><span data-stu-id="e2b06-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="e2b06-117">Để biết thêm thông tin, xem [kiểm tra các loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="e2b06-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="e2b06-118">**Báo cáo**</span><span class="sxs-lookup"><span data-stu-id="e2b06-118">**Reports**</span></span>
  
- <span data-ttu-id="e2b06-119">Nhận thông tin chi tiết dữ liệu nhạy cảm với [báo cáo DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="e2b06-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="e2b06-120">Xem chi tiết cụ thể của sự kiện với [báo cáo](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)việc làm.</span><span class="sxs-lookup"><span data-stu-id="e2b06-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
