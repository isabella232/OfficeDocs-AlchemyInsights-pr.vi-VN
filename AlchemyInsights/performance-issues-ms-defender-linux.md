---
title: Sự cố về hiệu suất đối với Microsoft Defender dành cho Điểm cuối trên Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794221"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="f28a4-102">Sự cố về hiệu suất đối với Microsoft Defender dành cho Điểm cuối trên Linux</span><span class="sxs-lookup"><span data-stu-id="f28a4-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="f28a4-103">Bài viết này hướng dẫn bạn qua các bước xác định sự cố hiệu suất cho Microsoft Defender dành cho Điểm cuối trên Linux.</span><span class="sxs-lookup"><span data-stu-id="f28a4-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="f28a4-104">Điều quan trọng là trước tiên phải xác minh rằng vấn đề mà bạn đang gặp phải được giải quyết bằng phiên [bản mới nhất.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="f28a4-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="f28a4-105">Để bắt đầu điều tra, hãy xem mục [Khắc phục sự cố về hiệu suất cho Microsoft Defender dành cho Điểm cuối trên Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span><span class="sxs-lookup"><span data-stu-id="f28a4-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="f28a4-106">Loại trừ</span><span class="sxs-lookup"><span data-stu-id="f28a4-106">Exclusions</span></span>

<span data-ttu-id="f28a4-107">Loại trừ có thể giúp giảm thiểu sự cố về hiệu suất.</span><span class="sxs-lookup"><span data-stu-id="f28a4-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="f28a4-108">Hãy xem lại các mục loại trừ trước khi bắt đầu để biết và ghi nhận mọi rủi ro bổ sung.</span><span class="sxs-lookup"><span data-stu-id="f28a4-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="f28a4-109">Để biết thêm thông tin, hãy xem mục Đặt cấu hình và xác thực các mục loại trừ [cho Bộ bảo vệ Microsoft dành cho Điểm cuối trên Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="f28a4-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="f28a4-110">Khi bạn có nhiều tệp và & mục cần loại trừ và tất cả đều nằm ở cùng một điểm gắn kết, việc loại trừ điểm gắn có có thể sẽ dễ dàng hơn.</span><span class="sxs-lookup"><span data-stu-id="f28a4-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="f28a4-111">Bắt đầu từ bản phát hành Tháng Hai 101.22.80, bạn có thể loại trừ toàn bộ điểm gắn kết.</span><span class="sxs-lookup"><span data-stu-id="f28a4-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="f28a4-112">Ví dụ: nếu /mnt/backup là một mountpoint, bạn có thể thêm /mnt/backup vào danh sách loại trừ bằng cách chạy lệnh này:</span><span class="sxs-lookup"><span data-stu-id="f28a4-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="f28a4-113">**Lưu** ý: Việc thêm loại trừ sẽ làm tăng nguy cơ không phát hiện phần mềm xấu, đồng thời cần được xử lý và thực hiện một cách cẩn thận.</span><span class="sxs-lookup"><span data-stu-id="f28a4-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="f28a4-114">Bạn cần Trợ giúp?</span><span class="sxs-lookup"><span data-stu-id="f28a4-114">Need Help?</span></span>

<span data-ttu-id="f28a4-115">Để hỗ trợ bạn một cách hiệu quả nhất, hãy thu thập dữ liệu chẩn đoán trước khi mở một trường hợp hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="f28a4-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
