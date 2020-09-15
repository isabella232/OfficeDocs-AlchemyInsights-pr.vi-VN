---
title: Quy tắc định đối với SSN không hoạt động
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679391"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="5cf1b-102">Các vấn đề về số an sinh xã hội</span><span class="sxs-lookup"><span data-stu-id="5cf1b-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="5cf1b-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="5cf1b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="5cf1b-104">**Các vấn đề về việc có SSNs**</span><span class="sxs-lookup"><span data-stu-id="5cf1b-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="5cf1b-105">Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung chứa **số an sinh xã hội (SSN)** khi sử dụng kiểu thông tin nhạy cảm trong Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="5cf1b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="5cf1b-106">Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="5cf1b-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="5cf1b-107">Ví dụ: đối với một chính sách SSN được cấu hình với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="5cf1b-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="5cf1b-108">**[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 chữ số, trong đó có thể có trong một mẫu có định dạng hoặc chưa định dạng</span><span class="sxs-lookup"><span data-stu-id="5cf1b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="5cf1b-109">**[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn hàm Look cho SSNs trong bốn mẫu khác nhau:</span><span class="sxs-lookup"><span data-stu-id="5cf1b-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="5cf1b-110">Func_ssn tìm thấy các SSNs với định dạng mạnh 2011 được định dạng bằng dấu gạch ngang hoặc dấu cách (DDD-dd-dddd hoặc DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="5cf1b-111">Func_unformatted_ssn tìm thấy các SSNs với định dạng mạnh 2011 được bỏ định dạng dưới dạng chín chữ số liên tiếp (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="5cf1b-112">Func_randomized_formatted_ssn tìm thấy Post-2011 SSNs được định dạng bằng dấu gạch ngang hoặc dấu cách (DDD-dd-dddd hoặc DDD dd dddd)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="5cf1b-113">Func_randomized_unformatted_ssn tìm thấy Post-2011 SSNs không được định dạng dưới dạng chín chữ số liên tiếp (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="5cf1b-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="5cf1b-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="5cf1b-115">**[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Chính sách có thể là 85% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="5cf1b-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="5cf1b-116">[Hàm Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) tìm thấy nội dung khớp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="5cf1b-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="5cf1b-117">Tìm thấy một từ khóa từ [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="5cf1b-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="5cf1b-118">Ví dụ về từ khóa bao gồm:  *an sinh xã hội, số an sinh xã hội #, SoC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="5cf1b-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="5cf1b-119">Ví dụ, mẫu sau sẽ được kích hoạt cho chính sách định vị: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="5cf1b-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="5cf1b-120">Để biết thêm thông tin về những điều cần thiết cho SSNs được phát hiện đối với nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm cần tìm kiếm SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="5cf1b-121">Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="5cf1b-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  