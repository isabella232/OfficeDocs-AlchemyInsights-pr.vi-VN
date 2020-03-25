---
title: DLP chính sách Mẹo không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932608"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="2b8a7-102">DLP chính sách Mẹo vấn đề</span><span class="sxs-lookup"><span data-stu-id="2b8a7-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="2b8a7-103">**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="2b8a7-104">Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="2b8a7-105">Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="2b8a7-106">Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="2b8a7-107">Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="2b8a7-108">Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="2b8a7-109">**Mẹo DLP chính sách**</span><span class="sxs-lookup"><span data-stu-id="2b8a7-109">**DLP policy tips**</span></span>

<span data-ttu-id="2b8a7-110">Khi sử dụng **chính sách DLP**, người dùng có thể được thông báo về vi phạm chính sách với **Mẹo chính sách**.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="2b8a7-111">Quản trị viên có thể cấu hình chính sách Mẹo để hiển thị trong khi kiểm tra chính sách DLP hoặc khi chính sách ở chế độ thực thi đầy đủ.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="2b8a7-112">Cấu hình chính sách Mẹo trên chính sách DLP của bạn trong Trung tâm bảo mật và tuân thủ trong chế độ thực thi đầy đủ, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="2b8a7-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="2b8a7-113">Đảm bảo chính sách Mẹo đã được **kích hoạt** trên quy tắc DLP bằng cách sử dụng các bước tại [đây](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="2b8a7-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="2b8a7-114">Đảm bảo **nội dung** của bạn phù hợp với những gì **cần thiết** để kích hoạt quy tắc được nêu trong bài viết này ở [đây](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2b8a7-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2b8a7-115">Chính sách Mẹo Hiển thị trong OWA và Outlook.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="2b8a7-116">Tuy nhiên, khi sử dụng **Outlook 2013 hoặc mới**hơn, Mẹo chính sách chỉ hiển thị trong một số điều kiện.</span><span class="sxs-lookup"><span data-stu-id="2b8a7-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="2b8a7-117">Các điều kiện được liệt kê ở đây: [điều kiện được hỗ trợ cho Outlook 2013 hoặc mới hơn để hiển thị Mẹo chính sách](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="2b8a7-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="2b8a7-118">Để biết thêm thông tin về chính sách DLP Mẹo, xem: [Hiển thị chính sách Mẹo DLP chính](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips) sách</span><span class="sxs-lookup"><span data-stu-id="2b8a7-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  