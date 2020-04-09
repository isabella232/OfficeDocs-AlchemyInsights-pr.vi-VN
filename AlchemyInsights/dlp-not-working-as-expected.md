---
title: DLP không hoạt động như mong đợi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977460"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="22ae4-102">DLP không hoạt động như mong đợi</span><span class="sxs-lookup"><span data-stu-id="22ae4-102">DLP not working as expected</span></span>

<span data-ttu-id="22ae4-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="22ae4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="22ae4-104">**Thiết lập DLP**</span><span class="sxs-lookup"><span data-stu-id="22ae4-104">**Setting up DLP**</span></span>

<span data-ttu-id="22ae4-105">Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** trong Office 365 không hoạt động như mong đợi?</span><span class="sxs-lookup"><span data-stu-id="22ae4-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="22ae4-106">Nếu có, đảm bảo rằng **chính sách DLP** của bạn được thiết lập chính xác và dữ liệu của bạn chứa những gì **chính sách DLP** đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="22ae4-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="22ae4-107">Chính sách DLP cho phép bạn xác định và bảo vệ thông tin nhạy cảm trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="22ae4-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="22ae4-108">Thiết lập chính sách DLP, sử dụng thông tin [ở đây](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="22ae4-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="22ae4-109">**Chính sách DLP nào tìm kiếm**</span><span class="sxs-lookup"><span data-stu-id="22ae4-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="22ae4-110">Khi sử dụng các **loại thông tin nhạy cảm tích hợp** trong Office 365 Trung tâm bảo mật và tuân thủ, chính sách DLP tìm các mẫu và yếu tố cụ thể khi phát hiện các loại nhạy cảm.</span><span class="sxs-lookup"><span data-stu-id="22ae4-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="22ae4-111">**Tích hợp các loại thông tin nhạy cảm**</span><span class="sxs-lookup"><span data-stu-id="22ae4-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="22ae4-112">Để biết thông tin về các loại nhạy cảm và chính sách DLP sẽ tìm kiếm khi phát hiện loại nhạy cảm, hãy xem: [những loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="22ae4-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="22ae4-113">**Các loại thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="22ae4-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="22ae4-114">Nếu bạn đang cố gắng tạo các loại thông tin nhạy cảm tùy chỉnh, hãy sử dụng bài viết sau để biết thông tin về cách tạo loại nhạy cảm tùy chỉnh: [tạo loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="22ae4-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="22ae4-115">**Kiểm tra chính sách DLP**</span><span class="sxs-lookup"><span data-stu-id="22ae4-115">**Test a DLP policy**</span></span>

<span data-ttu-id="22ae4-116">Để kiểm tra dữ liệu của bạn bằng loại thông tin nhạy cảm được tích hợp hoặc tùy chỉnh, hãy **Classifications** > sử dụng tùy chọn **loại thử nghiệm** trong phân**loại thông tin nhạy cảm**.</span><span class="sxs-lookup"><span data-stu-id="22ae4-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="22ae4-117">Để biết thêm thông tin, xem [kiểm tra các loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="22ae4-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="22ae4-118">**Báo cáo**</span><span class="sxs-lookup"><span data-stu-id="22ae4-118">**Reports**</span></span>
  
- <span data-ttu-id="22ae4-119">Nhận thông tin chi tiết dữ liệu nhạy cảm với [báo cáo DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="22ae4-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="22ae4-120">Xem chi tiết cụ thể của sự kiện với [báo cáo](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)việc làm.</span><span class="sxs-lookup"><span data-stu-id="22ae4-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
