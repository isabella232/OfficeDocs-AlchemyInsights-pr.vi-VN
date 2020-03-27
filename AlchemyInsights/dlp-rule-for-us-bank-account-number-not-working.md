---
title: Quy tắc DLP cho số tài khoản ngân hàng Hoa Kỳ không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977184"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="15f19-102">Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ</span><span class="sxs-lookup"><span data-stu-id="15f19-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="15f19-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="15f19-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="15f19-104">**Vấn đề DLP với số tài khoản ngân hàng của Hoa Kỳ**</span><span class="sxs-lookup"><span data-stu-id="15f19-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="15f19-105">Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số tài khoản ngân hàng Hoa Kỳ** khi sử dụng loại thông tin nhạy cảm DLP trong O365?</span><span class="sxs-lookup"><span data-stu-id="15f19-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="15f19-106">Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="15f19-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="15f19-107">Ví dụ: đối với chính sách **số tài khoản ngân hàng Hoa Kỳ** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="15f19-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="15f19-108">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 chữ số</span><span class="sxs-lookup"><span data-stu-id="15f19-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="15f19-109">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 chữ số liên tiếp.</span><span class="sxs-lookup"><span data-stu-id="15f19-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="15f19-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="15f19-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="15f19-111">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="15f19-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="15f19-112">Biểu thức chính thông Regex_usa_bank_account_number tìm thấy nội dung phù hợp với mẫu</span><span class="sxs-lookup"><span data-stu-id="15f19-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="15f19-113">Tìm thấy từ khóa từ Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="15f19-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="15f19-114">Ví dụ, mẫu sau đây có kích hoạt cho chính sách **số tài khoản ngân hàng Hoa Kỳ** : kiểm tra tài khoản 78344011</span><span class="sxs-lookup"><span data-stu-id="15f19-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="15f19-115">Để biết thêm thông tin về những gì được yêu cầu cho một **số tài khoản ngân hàng Hoa Kỳ** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm kiếm số tài khoản ngân hàng Hoa Kỳ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="15f19-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="15f19-116">Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="15f19-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  