---
title: Quy tắc số thẻ tín dụng không hoạt động
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679463"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="6edfb-102">Các vấn đề về các số thẻ tín dụng</span><span class="sxs-lookup"><span data-stu-id="6edfb-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="6edfb-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="6edfb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6edfb-104">**Các vấn đề về các số thẻ tín dụng**</span><span class="sxs-lookup"><span data-stu-id="6edfb-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="6edfb-105">Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung chứa một **số thẻ tín dụng** khi sử dụng kiểu thông tin nhạy cảm trong O365?</span><span class="sxs-lookup"><span data-stu-id="6edfb-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="6edfb-106">Nếu vậy, hãy đảm bảo rằng nội dung của bạn có chứa thông tin cần thiết để kích hoạt chính sách được phát hiện khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="6edfb-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="6edfb-107">Ví dụ: đối với một **chính sách thẻ tín dụng** được cấu hình với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="6edfb-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="6edfb-108">**[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 chữ số có thể được định dạng hoặc không được định dạng (dddddddddddddddddddddddd) và phải vượt qua kiểm tra Luhn.</span><span class="sxs-lookup"><span data-stu-id="6edfb-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="6edfb-109">**[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Mẫu rất phức tạp và mạnh mẽ mà phát hiện thẻ từ tất cả các thương hiệu lớn trên toàn thế giới, bao gồm Visa, MasterCard, Discover Card, JCB, American Express, Gift Cards và Diner cards.</span><span class="sxs-lookup"><span data-stu-id="6edfb-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="6edfb-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Có, checksum Luhn</span><span class="sxs-lookup"><span data-stu-id="6edfb-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="6edfb-111">**[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Chính sách có thể là 85% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="6edfb-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="6edfb-112">Hàm Func_credit_card tìm thấy nội dung khớp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="6edfb-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="6edfb-113">Một trong những điều sau là đúng:</span><span class="sxs-lookup"><span data-stu-id="6edfb-113">One of the following is true:</span></span>

  - <span data-ttu-id="6edfb-114">Tìm thấy một từ khóa từ Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="6edfb-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="6edfb-115">Một từ khóa từ Keyword_cc_name được tìm thấy</span><span class="sxs-lookup"><span data-stu-id="6edfb-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="6edfb-116">Hàm Func_expiration_date tìm thấy một ngày trong định dạng ngày bên phải.</span><span class="sxs-lookup"><span data-stu-id="6edfb-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="6edfb-117">Bộ kiểm tra vượt quá</span><span class="sxs-lookup"><span data-stu-id="6edfb-117">The checksum passes</span></span>

    <span data-ttu-id="6edfb-118">Ví dụ, mẫu sau sẽ kích hoạt cho chính sách số thẻ tín dụng đã định vị:</span><span class="sxs-lookup"><span data-stu-id="6edfb-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="6edfb-119">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="6edfb-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="6edfb-120">Hết hạn: 2/2009</span><span class="sxs-lookup"><span data-stu-id="6edfb-120">Expires: 2/2009</span></span>

<span data-ttu-id="6edfb-121">Để biết thêm thông tin về yêu cầu **số thẻ tín dụng** được phát hiện đối với nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm cần tìm kiếm thẻ tín dụng #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="6edfb-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="6edfb-122">Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="6edfb-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  