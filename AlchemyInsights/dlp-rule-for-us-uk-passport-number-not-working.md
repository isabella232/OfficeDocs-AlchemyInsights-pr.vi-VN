---
title: Quy tắc không hoạt động cho số hộ chiếu US/Vương Quốc Anh
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679246"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c5352-102">Các vấn đề với số lượng hộ chiếu US/UK</span><span class="sxs-lookup"><span data-stu-id="c5352-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c5352-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="c5352-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c5352-104">**Phát sinh các vấn đề với số hộ chiếu US/Vương Quốc Anh**</span><span class="sxs-lookup"><span data-stu-id="c5352-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c5352-105">Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung có chứa một **số hộ chiếu US/UK** khi sử dụng loại thông tin nhạy cảm trong O365?</span><span class="sxs-lookup"><span data-stu-id="c5352-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c5352-106">Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="c5352-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c5352-107">Ví dụ: đối với một chính sách **số Passport US/UK** được cấu hình với mức độ tin cậy của 75%, các thao tác sau được đánh giá và phải được phát hiện cho quy tắc kích hoạt</span><span class="sxs-lookup"><span data-stu-id="c5352-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c5352-108">**[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Chín chữ số</span><span class="sxs-lookup"><span data-stu-id="c5352-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="c5352-109">**[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Chín chữ số liên tiếp</span><span class="sxs-lookup"><span data-stu-id="c5352-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c5352-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="c5352-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c5352-111">**[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Chính sách có thể là 75% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="c5352-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c5352-112">Hàm Func_usa_uk_passport tìm thấy nội dung khớp với mẫu.</span><span class="sxs-lookup"><span data-stu-id="c5352-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c5352-113">Tìm thấy một từ khóa từ Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c5352-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c5352-114">Ví dụ, mẫu sau đây sẽ kích hoạt cho chính sách **số hộ chiếu Hoa Kỳ/Vương Quốc Anh** : số hộ chiếu hoa kỳ 123456789</span><span class="sxs-lookup"><span data-stu-id="c5352-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c5352-115">Để biết thêm thông tin về những điều cần thiết đối với số hộ chiếu US/UK sẽ được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm nào tìm kiếm đối với số hộ chiếu US/Vương Quốc Anh](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c5352-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c5352-116">Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c5352-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  