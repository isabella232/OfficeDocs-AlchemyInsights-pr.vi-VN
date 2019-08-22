---
title: Quy tắc DLP SSN không làm việc
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529900"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="91f39-102">DLP các vấn đề với số an sinh xã hội</span><span class="sxs-lookup"><span data-stu-id="91f39-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="91f39-103">Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **Số an sinh xã hội (SSN)** khi sử dụng một loại thông tin nhạy cảm trong Office 365?</span><span class="sxs-lookup"><span data-stu-id="91f39-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="91f39-104">Nếu vậy, hãy chắc chắn rằng nội dung của bạn có chứa các thông tin cần thiết cho chính sách DLP là đang tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="91f39-104">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="91f39-105">Ví dụ, cho một chính sách SSN, cấu hình với mức độ tin cậy là 85%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="91f39-105">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="91f39-106">9 **[định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** chữ số, có thể trong một mô hình định dạng hay định dạng</span><span class="sxs-lookup"><span data-stu-id="91f39-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="91f39-107">**[Mẫu:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Bốn chức năng tìm kiếm SSNs trong bốn mẫu khác nhau:</span><span class="sxs-lookup"><span data-stu-id="91f39-107">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="91f39-108">Func_ssn tìm thấy SSNs với pre-2011 mạnh định dạng được định dạng với dấu gạch ngang hoặc gian (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="91f39-108">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="91f39-109">Func_unformatted_ssn tìm thấy SSNs với pre-2011 mạnh định dạng được định dạng như chín chữ số liên tục (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="91f39-109">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="91f39-110">Func_randomized_formatted_ssn tìm thấy SSNs bài-2011 được định dạng với dấu gạch ngang hoặc gian (ddd-dd-dddd OR ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="91f39-110">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="91f39-111">Func_randomized_unformatted_ssn tìm thấy SSNs bài-2011 được định dạng như chín chữ số liên tục (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="91f39-111">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="91f39-112">**[Kiểm tra:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Không, đó là không có kiểm tra</span><span class="sxs-lookup"><span data-stu-id="91f39-112">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="91f39-113">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Một chính sách DLP là 85% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="91f39-113">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="91f39-114">[Chức năng Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) tìm thấy nội dung phù hợp với các mô hình.</span><span class="sxs-lookup"><span data-stu-id="91f39-114">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="91f39-115">Tìm thấy một từ khóa từ [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="91f39-115">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="91f39-116">Bao gồm các ví dụ của các từ khóa: *an sinh xã hội, an sinh xã hội #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="91f39-116">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="91f39-117">Ví dụ, các mẫu sau sẽ kích hoạt chính sách DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="91f39-117">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="91f39-118">Để biết thêm chi tiết về những gì là cần thiết cho SSNs phát hiện cho nội dung của bạn, hãy xem phần sau đây trong bài viết này: [Những gì the nhạy cảm loại thông tin tìm kiếm SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="91f39-118">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="91f39-119">Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="91f39-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  