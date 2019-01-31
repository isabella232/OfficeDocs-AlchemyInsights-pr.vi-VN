---
title: DLP quy tắc cho các số thẻ tín dụng không làm việc
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657489"
---
<span data-ttu-id="b94b0-p101">Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **Số thẻ tín dụng** khi sử dụng một loại thông tin nhạy cảm DLP trong O365? Nếu vậy, hãy chắc chắn rằng nội dung của bạn có chứa các thông tin cần thiết để kích hoạt các chính sách DLP khi nó được đánh giá. Ví dụ, cho một **thẻ tín dụng chính sách** được cấu hình với mức độ tin cậy là 85%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="b94b0-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="b94b0-105">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chữ số mà có thể được định dạng hoặc chưa định dạng (dddddddddddddddd) và phải vượt qua bài kiểm tra Luhn.</span><span class="sxs-lookup"><span data-stu-id="b94b0-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="b94b0-106">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Mô hình rất phức tạp và mạnh mẽ phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, Mastercard, Discover Card, JCB, American Express, thẻ quà tặng và quán ăn thẻ.</span><span class="sxs-lookup"><span data-stu-id="b94b0-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="b94b0-107">**[Kiểm tra:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Vâng, kiểm tra Luhn</span><span class="sxs-lookup"><span data-stu-id="b94b0-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="b94b0-108">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Một chính sách DLP là 85% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="b94b0-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="b94b0-109">Chức năng Func_credit_card tìm thấy nội dung phù hợp với các mô hình.</span><span class="sxs-lookup"><span data-stu-id="b94b0-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="b94b0-110">Một trong những điều sau đây là đúng:</span><span class="sxs-lookup"><span data-stu-id="b94b0-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="b94b0-111">Tìm thấy một từ khóa từ Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="b94b0-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="b94b0-112">Tìm thấy một từ khóa từ Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="b94b0-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="b94b0-113">Chức năng Func_expiration_date tìm thấy một ngày ở định dạng đúng ngày.</span><span class="sxs-lookup"><span data-stu-id="b94b0-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="b94b0-114">Đi kiểm tra</span><span class="sxs-lookup"><span data-stu-id="b94b0-114">The checksum passes</span></span>
    
    <span data-ttu-id="b94b0-115">Ví dụ, các mẫu sau sẽ kích hoạt cho một chính sách số DLP thẻ tín dụng:</span><span class="sxs-lookup"><span data-stu-id="b94b0-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="b94b0-116">Visa: 4485 3647 3952 7352 người</span><span class="sxs-lookup"><span data-stu-id="b94b0-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="b94b0-117">Hết hạn: tháng 2 năm 2009</span><span class="sxs-lookup"><span data-stu-id="b94b0-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="b94b0-118">Để biết thêm chi tiết về những gì là cần thiết cho một **Số thẻ tín dụng** để được phát hiện cho nội dung của bạn, hãy xem phần sau đây trong bài viết này: [Những gì the nhạy cảm loại thông tin tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b94b0-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b94b0-119">Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b94b0-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

