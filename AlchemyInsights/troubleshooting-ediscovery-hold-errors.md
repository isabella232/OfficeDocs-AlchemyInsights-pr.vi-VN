---
title: Khắc phục sự cố khám phá chứa lỗi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676532"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="d0907-102">Khắc phục sự cố khám phá chứa lỗi</span><span class="sxs-lookup"><span data-stu-id="d0907-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="d0907-103">Bạn gặp phải sự cố với việc lưu giữ Khám phá Điện tử?</span><span class="sxs-lookup"><span data-stu-id="d0907-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="d0907-104">Dưới đây là một số cách thực hành tốt nhất cần xem xét:</span><span class="sxs-lookup"><span data-stu-id="d0907-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="d0907-105">Kiểm tra trạng thái phân phối giữ lại.</span><span class="sxs-lookup"><span data-stu-id="d0907-105">Check the hold distribution status.</span></span>  <span data-ttu-id="d0907-106">Nếu trạng thái là **Bật (Đang chờ)** hoặc **Tắt (Đang chờ xử lý),** hãy chờ phân phối giữ để hoàn tất.</span><span class="sxs-lookup"><span data-stu-id="d0907-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="d0907-107">Phối Khám phá Điện tử lưu giữ các bản cập nhật thành một yêu cầu hàng loạt duy nhất thay vì cập nhật chính sách nhiều lần cho từng giao dịch.</span><span class="sxs-lookup"><span data-stu-id="d0907-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="d0907-108">Chạy Set-CaseHoldPolicy <policyname> -RetryDistribution trong Powershell của Trung tâm Bảo mật và Tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="d0907-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="d0907-109">Để biết chi tiết, hãy [xem Kết nối tâm Bảo & Tuân thủ PowerShell](/powershell/exchange/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="d0907-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="d0907-110">Để biết các bước kiểm tra các thiết đặt này và các phương pháp tốt nhất bổ sung để giảm thiểu và giải quyết vấn đề giữ Lại Khám phá Điện [tử,](/microsoft-365/compliance/hold-distribution-errors)hãy xem Khắc phục sự cố lỗi giữ Khám phá Điện tử .</span><span class="sxs-lookup"><span data-stu-id="d0907-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="d0907-111">Để biết thông tin về cách khắc phục các sự cố Khám phá Điện tử phổ biến khác, hãy xem mục Điều tra, khắc phục sự cố và giải quyết các [sự cố Khám phá Điện tử thông thường.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="d0907-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
