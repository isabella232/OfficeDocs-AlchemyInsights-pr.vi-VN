---
title: Quy tắc DLP cho số thẻ tín dụng không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704223"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="ad466-102">DLP vấn đề với số thẻ tín dụng</span><span class="sxs-lookup"><span data-stu-id="ad466-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="ad466-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="ad466-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="ad466-104">**DLP vấn đề với số thẻ tín dụng**</span><span class="sxs-lookup"><span data-stu-id="ad466-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="ad466-105">Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa **số thẻ tín dụng** khi sử dụng loại thông tin nhạy cảm DLP trong O365?</span><span class="sxs-lookup"><span data-stu-id="ad466-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="ad466-106">Nếu có, đảm bảo rằng nội dung của bạn chứa thông tin cần thiết để kích hoạt chính sách DLP khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="ad466-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="ad466-107">Ví dụ: đối với **chính sách thẻ tín dụng** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="ad466-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="ad466-108">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chữ số mà có thể được định dạng hoặc định dạng (dddddddddddddddd) và phải vượt qua các thử nghiệm Luhn.</span><span class="sxs-lookup"><span data-stu-id="ad466-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="ad466-109">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Rất phức tạp và mạnh mẽ mô hình phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, thẻ quà tặng, và thẻ Diner.</span><span class="sxs-lookup"><span data-stu-id="ad466-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="ad466-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Có, kiểm tra Luhn</span><span class="sxs-lookup"><span data-stu-id="ad466-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="ad466-111">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Chính sách DLP là 85% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="ad466-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="ad466-112">Chức năng Func_credit_card tìm thấy nội dung phù hợp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="ad466-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="ad466-113">Một trong những việc sau đây là đúng:</span><span class="sxs-lookup"><span data-stu-id="ad466-113">One of the following is true:</span></span>

  - <span data-ttu-id="ad466-114">Một từ khóa từ Keyword_cc_verification được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="ad466-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="ad466-115">Một từ khóa từ Keyword_cc_name được tìm thấy</span><span class="sxs-lookup"><span data-stu-id="ad466-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="ad466-116">Chức năng Func_expiration_date tìm thấy một ngày ở định dạng ngày đúng.</span><span class="sxs-lookup"><span data-stu-id="ad466-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="ad466-117">Checksum đi qua</span><span class="sxs-lookup"><span data-stu-id="ad466-117">The checksum passes</span></span>

    <span data-ttu-id="ad466-118">Ví dụ, mẫu sau đây có kích hoạt cho chính sách số thẻ tín dụng DLP:</span><span class="sxs-lookup"><span data-stu-id="ad466-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="ad466-119">Thị thực: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="ad466-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="ad466-120">Hết hạn: 2/2009</span><span class="sxs-lookup"><span data-stu-id="ad466-120">Expires: 2/2009</span></span>

<span data-ttu-id="ad466-121">Để biết thêm thông tin về những gì được yêu cầu cho một **số thẻ tín dụng** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những gì các loại thông tin nhạy cảm tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="ad466-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="ad466-122">Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="ad466-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  