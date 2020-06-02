---
title: Quy tắc DLP cho SSN không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507392"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="bb691-102">Các vấn đề DLP với số an ninh xã hội</span><span class="sxs-lookup"><span data-stu-id="bb691-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="bb691-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="bb691-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="bb691-104">**Vấn đề DLP với SSNs**</span><span class="sxs-lookup"><span data-stu-id="bb691-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="bb691-105">Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** không hoạt động cho nội dung có chứa **số an ninh xã hội (SSN)** khi sử dụng loại thông tin nhạy cảm trong Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="bb691-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="bb691-106">Nếu vậy, hãy đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="bb691-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="bb691-107">Ví dụ: đối với một chính sách SSN được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="bb691-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="bb691-108">**[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 chữ số, trong đó có thể là một mẫu định dạng</span><span class="sxs-lookup"><span data-stu-id="bb691-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="bb691-109">**[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn chức năng tìm kiếm SSNs trong bốn mô hình khác nhau:</span><span class="sxs-lookup"><span data-stu-id="bb691-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="bb691-110">Func_ssn thấy SSNs với Pre-2011 định dạng mạnh được định dạng với dấu gạch ngang hoặc không gian (DDD-dd-dddd hoặc DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="bb691-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="bb691-111">Func_unformatted_ssn tìm thấy SSNs với Pre-2011 định dạng mạnh mẽ mà không thể bỏ là chín chữ số liên tiếp (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="bb691-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="bb691-112">Func_randomized_formatted_ssn tìm thấy bài viết-2011 SSNs được định dạng với dấu gạch ngang hoặc không gian (DDD-dd-dddd hoặc DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="bb691-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="bb691-113">Func_randomized_unformatted_ssn tìm thấy bài đăng-2011 SSNs được định dạng là chín chữ số liên tiếp (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="bb691-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="bb691-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="bb691-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="bb691-115">**[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Chính sách DLP là 85% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="bb691-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="bb691-116">[Chức năng Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) tìm thấy nội dung phù hợp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="bb691-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="bb691-117">Từ khóa từ [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="bb691-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="bb691-118">Ví dụ về các từ khóa bao gồm: *an ninh xã hội, an ninh xã hội #, SoC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="bb691-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="bb691-119">Ví dụ, mẫu sau đây có kích hoạt cho chính sách DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="bb691-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="bb691-120">Để biết thêm thông tin về những gì được yêu cầu cho SSNs được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm kiếm SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="bb691-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="bb691-121">Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="bb691-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  