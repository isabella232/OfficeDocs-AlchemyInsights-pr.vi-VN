---
title: DLP quy tắc cho Hoa Kỳ / Vương Quốc Anh số hộ chiếu không làm việc
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: ec7f11676982b56a46c83bf276c2212ce765ba6f
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786720"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="be910-102">Vấn đề với DLP - U.S. / UK hộ chiếu số</span><span class="sxs-lookup"><span data-stu-id="be910-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="be910-p101">Bạn đang gặp vấn đề với **Công tác phòng chống mất mát dữ liệu (DLP)** không làm việc cho nội dung có chứa một **U.S. / số hộ chiếu Anh Quốc** khi sử dụng một loại thông tin nhạy cảm DLP trong O365? Nếu vậy, hãy chắc chắn rằng nội dung của bạn sẽ chứa các thông tin cần thiết cho những gì chính sách DLP tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="be910-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="be910-105">Ví dụ, cho một **U.S. / số hộ chiếu của Anh** chính sách được cấu hình với mức độ tin cậy của 75%, sau đây được đánh giá và phải được phát hiện cho quy tắc để kích hoạt</span><span class="sxs-lookup"><span data-stu-id="be910-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="be910-106">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 chữ số</span><span class="sxs-lookup"><span data-stu-id="be910-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="be910-107">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 chữ số liên tục</span><span class="sxs-lookup"><span data-stu-id="be910-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="be910-108">**[Kiểm tra:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, đó là không có kiểm tra</span><span class="sxs-lookup"><span data-stu-id="be910-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="be910-109">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Một chính sách DLP là 75% tự tin rằng nó đã phát hiện đây là loại thông tin nhạy cảm nếu, trong vòng một gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="be910-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="be910-110">Chức năng Func_usa_uk_passport tìm thấy nội dung phù hợp với các mô hình.</span><span class="sxs-lookup"><span data-stu-id="be910-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="be910-111">Tìm thấy một từ khóa từ Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="be910-111">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="be910-112">Ví dụ, các mẫu sau sẽ kích hoạt cho các **U.S. / số hộ chiếu Anh Quốc** sách: hộ chiếu Hoa Kỳ số 123456789</span><span class="sxs-lookup"><span data-stu-id="be910-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="be910-113">Để biết thêm về những gì là cần thiết cho một Mỹ / số hộ chiếu Anh Quốc để được phát hiện cho nội dung của bạn, xem phần sau đây trong bài viết này: [xem xét những gì the nhạy cảm thông tin loại cho Hoa Kỳ / số hộ chiếu Anh Quốc](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="be910-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="be910-114">Bằng cách sử dụng một loại thông tin nhạy cảm khác nhau được xây dựng trong, xem bài viết sau đây để có thông tin về những gì là cần thiết cho các loại khác: [những gì the nhạy cảm loại thông tin tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="be910-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

