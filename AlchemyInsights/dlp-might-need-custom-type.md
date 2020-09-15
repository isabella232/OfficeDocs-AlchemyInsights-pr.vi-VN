---
title: Có thể cần một kiểu tùy chỉnh
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712206"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="51079-102">Có thể cần một kiểu tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="51079-102">DLP might need a custom type</span></span>

<span data-ttu-id="51079-103">**Quan trọng**: trong những thời gian chưa từng có này, chúng tôi sẽ thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn sẵn có – vui lòng truy cập vào các điều [chỉnh tính năng tạm thời trong SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="51079-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="51079-104">**Có thể yêu cầu kiểu thông tin tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="51079-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="51079-105">Với chính sách ngăn ngừa mất dữ liệu (), bạn có thể xác định và bảo vệ dữ liệu nhạy cảm trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="51079-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="51079-106">Trong một số trường hợp, bạn có thể cần phải tạo kiểu thông tin nhạy cảm **tùy chỉnh** của riêng bạn để bảo vệ dữ liệu của tổ chức bạn.</span><span class="sxs-lookup"><span data-stu-id="51079-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="51079-107">Ví dụ, tổ chức của bạn có thể cần phải xác định và bảo vệ ID nhân viên hoặc dữ liệu khác ở một số định dạng cụ thể với tổ chức của bạn. Nếu vậy, hãy xem các bài viết sau để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="51079-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="51079-108">**Tùy chỉnh kiểu thông tin nhạy cảm tích hợp sẵn**</span><span class="sxs-lookup"><span data-stu-id="51079-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="51079-109">Nếu kiểu thông tin nhạy cảm tích hợp sẵn sẽ đáp ứng nhu cầu của bạn chỉ với một vài tinh chỉnh, bạn có thể [tùy chỉnh một kiểu thông tin được tích hợp sẵn](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="51079-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="51079-110">Ví dụ, bạn có thể thêm hoặc loại bỏ từ khóa hoặc thêm hoặc loại bỏ các bằng chứng hỗ trợ, chẳng hạn như ngày hoặc địa chỉ.</span><span class="sxs-lookup"><span data-stu-id="51079-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="51079-111">**Tạo kiểu thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="51079-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="51079-112">Tuy nhiên, nếu bạn cần xác định và bảo vệ một loại thông tin nhạy cảm khác, bạn có thể [tạo một kiểu thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) trong giao diện người dùng của Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="51079-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="51079-113">**Tạo kiểu thông tin nhạy cảm tùy chỉnh trong Trung tâm tuân thủ bảo mật & PowerShell**</span><span class="sxs-lookup"><span data-stu-id="51079-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="51079-114">Cuối cùng, nếu giao diện người dùng không cung cấp tất cả các tùy chọn bạn cần, bạn có thể [tạo kiểu thông tin nhạy cảm tùy chỉnh trong Trung tâm tuân thủ bảo mật & PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="51079-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="51079-115">Bằng cách bắt đầu với tệp XML, bạn có thể sử dụng mọi tùy chọn sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="51079-115">By starting with an XML file, you can use every option available.</span></span>
