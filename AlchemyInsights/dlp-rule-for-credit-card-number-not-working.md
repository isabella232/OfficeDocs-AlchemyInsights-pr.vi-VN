---
title: Quy tắc DLP cho số thẻ tín dụng không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932465"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="c0b3c-102">DLP vấn đề với số thẻ tín dụng</span><span class="sxs-lookup"><span data-stu-id="c0b3c-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="c0b3c-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="c0b3c-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="c0b3c-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="c0b3c-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="c0b3c-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="c0b3c-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="c0b3c-109">**DLP vấn đề với số thẻ tín dụng**</span><span class="sxs-lookup"><span data-stu-id="c0b3c-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="c0b3c-110">Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa **số thẻ tín dụng** khi sử dụng loại thông tin nhạy cảm DLP trong O365?</span><span class="sxs-lookup"><span data-stu-id="c0b3c-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c0b3c-111">Nếu có, đảm bảo rằng nội dung của bạn chứa thông tin cần thiết để kích hoạt chính sách DLP khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="c0b3c-112">Ví dụ: đối với **chính sách thẻ tín dụng** được cấu hình với mức độ tin cậy là 85%, sau đây là đánh giá và phải được phát hiện để quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="c0b3c-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="c0b3c-113">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 chữ số mà có thể được định dạng hoặc định dạng (dddddddddddddddd) và phải vượt qua các thử nghiệm Luhn.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="c0b3c-114">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Rất phức tạp và mạnh mẽ mô hình phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, thẻ quà tặng, và thẻ Diner.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="c0b3c-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Có, kiểm tra Luhn</span><span class="sxs-lookup"><span data-stu-id="c0b3c-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="c0b3c-116">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Chính sách DLP là 85% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="c0b3c-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c0b3c-117">Chức năng Func_credit_card tìm thấy nội dung phù hợp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c0b3c-118">Một trong những việc sau đây là đúng:</span><span class="sxs-lookup"><span data-stu-id="c0b3c-118">One of the following is true:</span></span>

  - <span data-ttu-id="c0b3c-119">Một từ khóa từ Keyword_cc_verification được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="c0b3c-120">Một từ khóa từ Keyword_cc_name được tìm thấy</span><span class="sxs-lookup"><span data-stu-id="c0b3c-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="c0b3c-121">Chức năng Func_expiration_date tìm thấy một ngày ở định dạng ngày đúng.</span><span class="sxs-lookup"><span data-stu-id="c0b3c-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="c0b3c-122">Checksum đi qua</span><span class="sxs-lookup"><span data-stu-id="c0b3c-122">The checksum passes</span></span>

    <span data-ttu-id="c0b3c-123">Ví dụ, mẫu sau đây có kích hoạt cho chính sách số thẻ tín dụng DLP:</span><span class="sxs-lookup"><span data-stu-id="c0b3c-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="c0b3c-124">Thị thực: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="c0b3c-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="c0b3c-125">Hết hạn: 2/2009</span><span class="sxs-lookup"><span data-stu-id="c0b3c-125">Expires: 2/2009</span></span>

<span data-ttu-id="c0b3c-126">Để biết thêm thông tin về những gì được yêu cầu cho một **số thẻ tín dụng** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những gì các loại thông tin nhạy cảm tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="c0b3c-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="c0b3c-127">Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c0b3c-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  