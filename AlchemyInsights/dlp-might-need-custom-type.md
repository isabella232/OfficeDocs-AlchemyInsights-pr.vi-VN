---
title: DLP có thể cần một loại tùy chỉnh
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704511"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="4e0c8-102">DLP có thể cần một loại tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="4e0c8-102">DLP might need a custom type</span></span>

<span data-ttu-id="4e0c8-103">**Quan trọng**: trong những lần chưa từng thấy, chúng tôi đang thực hiện các bước để đảm bảo rằng dịch vụ SharePoint Online và OneDrive vẫn có sẵn cao-vui lòng truy cập [điều chỉnh tính năng tạm thời của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4e0c8-104">**DLP có thể yêu cầu loại thông tin tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="4e0c8-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="4e0c8-105">Với chính sách ngăn chặn mất dữ liệu (DLP), bạn có thể xác định và bảo vệ dữ liệu nhạy cảm trong tổ chức của mình.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="4e0c8-106">Trong một số trường hợp, bạn có thể cần phải tạo loại thông tin nhạy cảm **tùy chỉnh** của riêng mình để bảo vệ dữ liệu của tổ chức.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="4e0c8-107">Ví dụ: tổ chức của bạn có thể cần phải xác định và bảo vệ ID nhân viên hoặc dữ liệu khác ở một số định dạng cụ thể cho sơ của bạn. Nếu có, hãy xem các bài viết sau để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="4e0c8-108">**Tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn**</span><span class="sxs-lookup"><span data-stu-id="4e0c8-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="4e0c8-109">Nếu một loại thông tin nhạy cảm được tích hợp sẵn đáp ứng nhu cầu của bạn chỉ bằng một vài tinh chỉnh, bạn có thể [tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="4e0c8-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="4e0c8-110">Ví dụ: bạn có thể thêm hoặc xóa từ khóa hoặc thêm hoặc xóa bằng chứng hỗ trợ như ngày hoặc địa chỉ.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="4e0c8-111">**Tạo loại thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="4e0c8-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="4e0c8-112">Nhưng nếu bạn cần xác định và bảo vệ một loại thông tin nhạy cảm khác nhau hoàn toàn, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) trong giao diện người dùng của Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="4e0c8-113">**Tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell**</span><span class="sxs-lookup"><span data-stu-id="4e0c8-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="4e0c8-114">Cuối cùng, nếu giao diện người dùng không cung cấp tất cả các tùy chọn bạn cần, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4e0c8-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="4e0c8-115">Bằng cách bắt đầu với một tập tin XML, bạn có thể sử dụng tất cả các tùy chọn có sẵn.</span><span class="sxs-lookup"><span data-stu-id="4e0c8-115">By starting with an XML file, you can use every option available.</span></span>
