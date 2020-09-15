---
title: Không hoạt động như mong đợi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679715"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="42aa0-102">Không hoạt động như mong đợi</span><span class="sxs-lookup"><span data-stu-id="42aa0-102">DLP not working as expected</span></span>

<span data-ttu-id="42aa0-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="42aa0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="42aa0-104">**Thiết lập có khoảng**</span><span class="sxs-lookup"><span data-stu-id="42aa0-104">**Setting up DLP**</span></span>

<span data-ttu-id="42aa0-105">Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** tiềm tàng) trong Office 365 không hoạt động như mong đợi?</span><span class="sxs-lookup"><span data-stu-id="42aa0-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="42aa0-106">Nếu vậy, hãy đảm bảo rằng **chính sách** của bạn được thiết lập đúng cách và dữ liệu của bạn có chứa nội **dung có thể** đang tìm kiếm khi nó đang được đánh giá hay không.</span><span class="sxs-lookup"><span data-stu-id="42aa0-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="42aa0-107">Các chính sách có thể cho phép bạn xác định và bảo vệ thông tin nhạy cảm trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="42aa0-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="42aa0-108">Để thiết lập chính sách đã có thể, hãy sử dụng thông tin [tại đây](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="42aa0-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="42aa0-109">**Giao diện chính sách nào cho**</span><span class="sxs-lookup"><span data-stu-id="42aa0-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="42aa0-110">Khi sử dụng các **kiểu thông tin nhạy cảm tích hợp sẵn** trong các trung tâm bảo mật và tuân thủ, các chính sách có diện mạo tìm kiếm các mẫu và thành phần cụ thể khi phát hiện các kiểu nhạy cảm này.</span><span class="sxs-lookup"><span data-stu-id="42aa0-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="42aa0-111">**Các kiểu thông tin nhạy cảm tích hợp sẵn**</span><span class="sxs-lookup"><span data-stu-id="42aa0-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="42aa0-112">Để biết thông tin về các kiểu nhạy cảm được tích hợp và nội dung của chính sách sẽ xảy ra khi phát hiện loại nhạy cảm, hãy xem: [Tìm hiểu xem các kiểu thông tin nhạy cảm gì](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="42aa0-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="42aa0-113">**Các kiểu thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="42aa0-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="42aa0-114">Nếu bạn đang cố gắng tạo kiểu thông tin nhạy cảm tùy chỉnh, hãy dùng bài viết sau để biết thông tin về cách tạo kiểu nhạy cảm tùy chỉnh: [tạo kiểu thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="42aa0-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="42aa0-115">**Kiểm tra chính sách có quy định**</span><span class="sxs-lookup"><span data-stu-id="42aa0-115">**Test a DLP policy**</span></span>

<span data-ttu-id="42aa0-116">Để kiểm tra dữ liệu của bạn với kiểu thông tin được tích hợp sẵn hoặc tùy chỉnh, hãy dùng tùy chọn **loại kiểm tra** **bên dưới phân**  >  **loại các kiểu thông tin nhạy cảm**.</span><span class="sxs-lookup"><span data-stu-id="42aa0-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="42aa0-117">Để biết thêm thông tin, hãy xem [kiểm tra các kiểu thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="42aa0-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="42aa0-118">**Báo cáo**</span><span class="sxs-lookup"><span data-stu-id="42aa0-118">**Reports**</span></span>
  
- <span data-ttu-id="42aa0-119">Nhận hiểu rõ dữ liệu nhạy cảm với các [báo cáo](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports) của tôi.</span><span class="sxs-lookup"><span data-stu-id="42aa0-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="42aa0-120">Xem chi tiết cụ thể của sự kiện với [báo cáo sự cố](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="42aa0-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
