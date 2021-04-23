---
title: Mẹo Chính sách của DLP không hoạt động
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958724"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="f24fd-102">Các sự cố về Mẹo Chính sách của DLP</span><span class="sxs-lookup"><span data-stu-id="f24fd-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="f24fd-103">**Quan** trọng: Trong những thời điểm chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng dịch vụ SharePoint Online và OneDrive luôn khả dụng cao – Vui lòng truy nhập Điều chỉnh Tính năng Tạm thời [của SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="f24fd-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f24fd-104">Để cấu hình mẹo chính sách về chính sách DLP của bạn trong trung tâm Bảo mật & Tuân thủ trong chế độ thực thi đầy đủ, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="f24fd-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="f24fd-105">Đảm bảo mẹo chính sách **đã được bật** trên quy tắc DLP.</span><span class="sxs-lookup"><span data-stu-id="f24fd-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="f24fd-106">Để biết các bước, hãy xem [Gửi thông báo email và hiển thị mẹo chính sách cho chính sách DLP.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="f24fd-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="f24fd-107">Đảm bảo nội dung của bạn khớp với những gì được yêu cầu để kích hoạt quy tắc được nêu trong định nghĩa thực thể [kiểu thông tin Nhạy cảm.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f24fd-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="f24fd-108">Mẹo chính sách hiển thị trong cả OWA và Outlook.</span><span class="sxs-lookup"><span data-stu-id="f24fd-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="f24fd-109">Tuy nhiên, khi dùng Outlook 2013 trở lên, các mẹo chính sách chỉ được hiển thị trong một số điều kiện nhất định.</span><span class="sxs-lookup"><span data-stu-id="f24fd-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="f24fd-110">Để biết danh sách điều kiện cụ thể, hãy [xem Các điều kiện được hỗ trợ cho Outlook 2013 trở lên để hiển thị Mẹo Chính sách.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="f24fd-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="f24fd-111">Để biết thông tin về mẹo Chính sách của DLP, hãy xem [Tham khảo mẹo](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) Chính sách của DLP và Ma trận Hỗ trợ cho [mẹo Chính sách của DLP.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="f24fd-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>