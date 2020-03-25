---
title: DLP có thể cần một loại tùy chỉnh
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932680"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="87209-102">DLP có thể cần một loại tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="87209-102">DLP might need a custom type</span></span>

<span data-ttu-id="87209-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="87209-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="87209-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="87209-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="87209-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="87209-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="87209-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="87209-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="87209-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="87209-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="87209-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="87209-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="87209-109">**DLP có thể yêu cầu loại thông tin tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="87209-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="87209-110">Với chính sách ngăn chặn mất dữ liệu (DLP), bạn có thể xác định và bảo vệ dữ liệu nhạy cảm trong tổ chức của mình.</span><span class="sxs-lookup"><span data-stu-id="87209-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="87209-111">Trong một số trường hợp, bạn có thể cần phải tạo loại thông tin nhạy cảm **tùy chỉnh** của riêng mình để bảo vệ dữ liệu của tổ chức.</span><span class="sxs-lookup"><span data-stu-id="87209-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="87209-112">Ví dụ: tổ chức của bạn có thể cần phải xác định và bảo vệ ID nhân viên hoặc dữ liệu khác ở một số định dạng cụ thể cho sơ của bạn. Nếu có, hãy xem các bài viết sau để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="87209-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="87209-113">**Tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn**</span><span class="sxs-lookup"><span data-stu-id="87209-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="87209-114">Nếu một loại thông tin nhạy cảm được tích hợp sẵn đáp ứng nhu cầu của bạn chỉ bằng một vài tinh chỉnh, bạn có thể [tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="87209-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="87209-115">Ví dụ: bạn có thể thêm hoặc xóa từ khóa hoặc thêm hoặc xóa bằng chứng hỗ trợ như ngày hoặc địa chỉ.</span><span class="sxs-lookup"><span data-stu-id="87209-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="87209-116">**Tạo loại thông tin nhạy cảm tùy chỉnh**</span><span class="sxs-lookup"><span data-stu-id="87209-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="87209-117">Nhưng nếu bạn cần xác định và bảo vệ một loại thông tin nhạy cảm khác nhau hoàn toàn, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) trong giao diện người dùng của Trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="87209-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="87209-118">**Tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell**</span><span class="sxs-lookup"><span data-stu-id="87209-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="87209-119">Cuối cùng, nếu giao diện người dùng không cung cấp tất cả các tùy chọn bạn cần, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="87209-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="87209-120">Bằng cách bắt đầu với một tập tin XML, bạn có thể sử dụng tất cả các tùy chọn có sẵn.</span><span class="sxs-lookup"><span data-stu-id="87209-120">By starting with an XML file, you can use every option available.</span></span>
