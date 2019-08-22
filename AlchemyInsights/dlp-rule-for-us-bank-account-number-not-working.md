---
title: DLP quy tắc cho chúng tôi tài khoản ngân hàng số không làm việc
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
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529905"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="fab7b-102">DLP các vấn đề với các con số tài khoản ngân hàng</span><span class="sxs-lookup"><span data-stu-id="fab7b-102">DLP issues with US Bank Account Numbers</span></span>

<span data-ttu-id="fab7b-103">Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **Số tài khoản ngân hàng của Mỹ** khi sử dụng một loại thông tin nhạy cảm DLP trong O365?</span><span class="sxs-lookup"><span data-stu-id="fab7b-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="fab7b-104">Nếu vậy, hãy chắc chắn rằng nội dung của bạn sẽ chứa các thông tin cần thiết cho những gì chính sách DLP tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="fab7b-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="fab7b-105">Ví dụ, đối với một **Số tài khoản ngân hàng Mỹ** chính sách được cấu hình với mức độ tin cậy là 85%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="fab7b-105">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="fab7b-106">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** chữ số 8-17</span><span class="sxs-lookup"><span data-stu-id="fab7b-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="fab7b-107">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** chữ số liên tục 8-17.</span><span class="sxs-lookup"><span data-stu-id="fab7b-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="fab7b-108">**[Kiểm tra:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, đó là không có kiểm tra</span><span class="sxs-lookup"><span data-stu-id="fab7b-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="fab7b-109">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** Một chính sách DLP là 75% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="fab7b-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="fab7b-110">Biểu hiện thường xuyên Regex_usa_bank_account_number tìm thấy nội dung phù hợp với các mô hình</span><span class="sxs-lookup"><span data-stu-id="fab7b-110">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="fab7b-111">Tìm thấy một từ khóa từ Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="fab7b-111">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="fab7b-112">Ví dụ, các mẫu sau sẽ kích hoạt chính sách **Hoa Kỳ tài khoản ngân hàng số** : kiểm tra tài khoản 78344011</span><span class="sxs-lookup"><span data-stu-id="fab7b-112">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="fab7b-113">Để biết thêm chi tiết về những gì là cần thiết cho một **Số tài khoản ngân hàng của Mỹ** để được phát hiện cho nội dung của bạn, hãy xem phần sau đây trong bài viết này: [Những gì the nhạy cảm loại thông tin tìm kiếm các số tài khoản ngân hàng Mỹ](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="fab7b-113">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="fab7b-114">Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fab7b-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  