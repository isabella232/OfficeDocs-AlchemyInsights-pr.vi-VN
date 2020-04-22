---
title: Quy tắc DLP cho US/UK Passport Number không làm việc
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 9d9615eccd1e245bf4ca32742bfc64321dd7a8cf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715008"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="cce9e-102">Vấn đề với DLP-US/Vương Quốc Anh số hộ chiếu</span><span class="sxs-lookup"><span data-stu-id="cce9e-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="cce9e-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="cce9e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="cce9e-104">**Các vấn đề DLP với số hộ chiếu Mỹ/Anh**</span><span class="sxs-lookup"><span data-stu-id="cce9e-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="cce9e-105">Bạn có vấn đề với **ngăn ngừa mất dữ liệu (DLP)** không làm việc cho nội dung có chứa một **số hộ chiếu Mỹ/Anh** khi sử dụng một loại thông tin nhạy cảm DLP trong O365?</span><span class="sxs-lookup"><span data-stu-id="cce9e-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="cce9e-106">Nếu có, đảm bảo nội dung của bạn chứa thông tin cần thiết cho chính sách DLP đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="cce9e-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="cce9e-107">Ví dụ: đối với một chính sách **số hộ chiếu Mỹ/Anh** được cấu hình với mức độ tin cậy 75%, sau đây là đánh giá và phải được phát hiện cho quy tắc kích hoạt</span><span class="sxs-lookup"><span data-stu-id="cce9e-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="cce9e-108">**[Định dạng:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Chín chữ số</span><span class="sxs-lookup"><span data-stu-id="cce9e-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="cce9e-109">**[Mẫu:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Chín số liên tiếp</span><span class="sxs-lookup"><span data-stu-id="cce9e-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="cce9e-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="cce9e-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="cce9e-111">**[Định nghĩa:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Chính sách DLP là 75% tự tin rằng nó được phát hiện loại thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="cce9e-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="cce9e-112">Chức năng Func_usa_uk_passport tìm thấy nội dung phù hợp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="cce9e-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="cce9e-113">Một từ khóa từ Keyword_passport được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="cce9e-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="cce9e-114">Ví dụ, mẫu sau đây kích hoạt cho **Hoa Kỳ/anh số hộ chiếu** chính sách: US passport Number 123456789</span><span class="sxs-lookup"><span data-stu-id="cce9e-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="cce9e-115">Để biết thêm thông tin về những gì được yêu cầu đối với một số hộ chiếu Mỹ/Anh được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những loại thông tin nhạy cảm tìm số hộ chiếu Hoa Kỳ/Vương Quốc Anh](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="cce9e-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="cce9e-116">Sử dụng loại thông tin nhạy cảm khác được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những gì được yêu cầu cho các loại khác: [các loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="cce9e-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  