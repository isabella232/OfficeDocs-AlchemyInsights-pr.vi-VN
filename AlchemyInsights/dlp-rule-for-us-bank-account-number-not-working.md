---
title: Quy tắc cho số tài khoản ngân hàng Hoa Kỳ không hoạt động
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679318"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="69c77-102">Các vấn đề về các số tài khoản ngân hàng Hoa Kỳ</span><span class="sxs-lookup"><span data-stu-id="69c77-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="69c77-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="69c77-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="69c77-104">**Các vấn đề về các số tài khoản ngân hàng Hoa Kỳ**</span><span class="sxs-lookup"><span data-stu-id="69c77-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="69c77-105">Bạn gặp sự cố với việc **ngăn ngừa mất dữ liệu (** đã cho) không hoạt động cho nội dung có chứa một **số tài khoản ngân hàng Hoa Kỳ** khi sử dụng kiểu thông tin nhạy cảm trong O365?</span><span class="sxs-lookup"><span data-stu-id="69c77-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="69c77-106">Nếu vậy, hãy đảm bảo nội dung của bạn có chứa thông tin cần thiết cho những gì chính sách có thể đang tìm kiếm khi nó được đánh giá.</span><span class="sxs-lookup"><span data-stu-id="69c77-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="69c77-107">Ví dụ: đối với một chính sách **số tài khoản ngân hàng Hoa Kỳ** với mức độ tin cậy của 85%, các thao tác sau được đánh giá và phải được phát hiện đối với quy tắc kích hoạt:</span><span class="sxs-lookup"><span data-stu-id="69c77-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="69c77-108">**[Định dạng:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 chữ số</span><span class="sxs-lookup"><span data-stu-id="69c77-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="69c77-109">**[Mẫu:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 chữ số liên tiếp.</span><span class="sxs-lookup"><span data-stu-id="69c77-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="69c77-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Không, không có checksum</span><span class="sxs-lookup"><span data-stu-id="69c77-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="69c77-111">**[Định nghĩa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Chính sách có thể là 75% tin cậy rằng nó phát hiện kiểu thông tin nhạy cảm này nếu, trong phạm vi gần 300 ký tự:</span><span class="sxs-lookup"><span data-stu-id="69c77-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="69c77-112">Biểu thức thông thường Regex_usa_bank_account_number tìm nội dung khớp với mẫu</span><span class="sxs-lookup"><span data-stu-id="69c77-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="69c77-113">Tìm thấy một từ khóa từ Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="69c77-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="69c77-114">Ví dụ, mẫu sau đây sẽ kích hoạt cho chính sách **số tài khoản ngân hàng Hoa Kỳ** : kiểm tra tài khoản 78344011</span><span class="sxs-lookup"><span data-stu-id="69c77-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="69c77-115">Để biết thêm thông tin về những điều cần thiết đối với **số tài khoản ngân hàng Hoa Kỳ** được phát hiện cho nội dung của bạn, hãy xem phần sau trong bài viết này: [những thông tin nhạy cảm nào tìm kiếm số tài khoản ngân hàng Hoa Kỳ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="69c77-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="69c77-116">Sử dụng loại thông tin nhạy cảm khác nhau được tích hợp sẵn, hãy xem bài viết sau để biết thông tin về những điều cần thiết đối với các loại khác: [Tìm hiểu xem những loại thông tin nhạy cảm](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="69c77-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  