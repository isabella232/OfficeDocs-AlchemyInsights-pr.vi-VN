---
title: Quy tắc giảm bề mặt tấn công
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676571"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="1d14c-102">Quy tắc giảm bề mặt tấn công</span><span class="sxs-lookup"><span data-stu-id="1d14c-102">Attack surface reduction rules</span></span>

<span data-ttu-id="1d14c-103">Loại trừ tệp hoặc thư mục có thể giảm nghiêm trọng bảo vệ do quy tắc giảm bề mặt tấn công cung cấp.</span><span class="sxs-lookup"><span data-stu-id="1d14c-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="1d14c-104">Các tệp đã bị quy tắc cho phép chạy sẽ bị chặn và không có báo cáo hoặc sự kiện nào được ghi lại.</span><span class="sxs-lookup"><span data-stu-id="1d14c-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="1d14c-105">Loại trừ áp dụng cho tất cả quy tắc cho phép loại trừ.</span><span class="sxs-lookup"><span data-stu-id="1d14c-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="1d14c-106">Loại trừ ASR sử dụng cùng một cú pháp như loại Tính năng Chống Virut của Bộ bảo vệ Microsoft loại trừ.</span><span class="sxs-lookup"><span data-stu-id="1d14c-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="1d14c-107">Để biết chi tiết, [hãy xem Cấu hình và xác thực loại trừ cho Tính năng Chống Virut của Bộ bảo vệ Microsoft quét.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="1d14c-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="1d14c-108">Để tránh vấn đề, [hãy xem lại Các lỗi phổ biến cần tránh khi xác định loại trừ.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="1d14c-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="1d14c-109">Không phải tất cả quy tắc ASR đều hỗ trợ loại trừ.</span><span class="sxs-lookup"><span data-stu-id="1d14c-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="1d14c-110">Để xác thực xem quy tắc của bạn có hỗ trợ loại trừ hay [không,](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)hãy xem bảng Các quy tắc giảm thiểu bề mặt tấn công .</span><span class="sxs-lookup"><span data-stu-id="1d14c-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="1d14c-111">Quy tắc giảm bề mặt tấn công</span><span class="sxs-lookup"><span data-stu-id="1d14c-111">Attack surface reduction rules</span></span>

<span data-ttu-id="1d14c-112">Bề mặt tấn công của tổ chức bao gồm tất cả những nơi mà kẻ tấn công có thể xâm phạm thiết bị hoặc mạng của tổ chức.</span><span class="sxs-lookup"><span data-stu-id="1d14c-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="1d14c-113">Giảm bề mặt tấn công của bạn đồng nghĩa với việc bảo vệ các thiết bị và mạng của tổ chức, điều này giúp những kẻ tấn công có ít cách thực hiện tấn công hơn.</span><span class="sxs-lookup"><span data-stu-id="1d14c-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="1d14c-114">Cấu hình quy tắc giảm thiểu bề mặt tấn công trong Bộ bảo vệ Microsoft dành cho Điểm cuối có thể giúp ích.</span><span class="sxs-lookup"><span data-stu-id="1d14c-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="1d14c-115">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="1d14c-115">For more information, see:</span></span>

- [<span data-ttu-id="1d14c-116">GUID quy tắc ánh xạ ASR thành tên</span><span class="sxs-lookup"><span data-stu-id="1d14c-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="1d14c-117">Yêu cầu về quy tắc ASR:</span><span class="sxs-lookup"><span data-stu-id="1d14c-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="1d14c-118">Windows 10 Pro, phiên bản 1709 trở lên</span><span class="sxs-lookup"><span data-stu-id="1d14c-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="1d14c-119">Windows 10 Enterprise, phiên bản 1709 trở lên</span><span class="sxs-lookup"><span data-stu-id="1d14c-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="1d14c-120">Windows Máy chủ, phiên bản 1803 (Kênh Nửa năm một lần) trở lên</span><span class="sxs-lookup"><span data-stu-id="1d14c-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="1d14c-121">Xác định loại trừ chính xác cần áp dụng</span><span class="sxs-lookup"><span data-stu-id="1d14c-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="1d14c-122">Tìm kiếm EVENTID 1121 hoặc 1122 trong Microsoft-Windows-Bộ bảo vệ Windows/Nhật ký hoạt động.</span><span class="sxs-lookup"><span data-stu-id="1d14c-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="1d14c-123">Đánh giá kịch bản và ngữ cảnh của khối và xác nhận rằng kịch bản này cần được bỏ chặn.</span><span class="sxs-lookup"><span data-stu-id="1d14c-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="1d14c-124">Đọc giá trị Đường dẫn trong chi tiết sự kiện, là giá trị xác định loại trừ.</span><span class="sxs-lookup"><span data-stu-id="1d14c-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="1d14c-125">Thực hiện loại trừ càng nghiêm ngặt càng tốt.</span><span class="sxs-lookup"><span data-stu-id="1d14c-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="1d14c-126">Áp dụng ký tự đại diện mà cần (ví dụ: thay thế biến Người dùng).</span><span class="sxs-lookup"><span data-stu-id="1d14c-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="1d14c-127">Áp dụng loại trừ theo nhu cầu triển khai của bạn.</span><span class="sxs-lookup"><span data-stu-id="1d14c-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="1d14c-128">Để biết chi tiết, xem mục [Tùy chỉnh quy tắc giảm thiểu bề mặt tấn công](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="1d14c-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="1d14c-129">Loại trừ không được thực hiện</span><span class="sxs-lookup"><span data-stu-id="1d14c-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="1d14c-130">Xác định quy tắc có hỗ trợ loại trừ hay không.</span><span class="sxs-lookup"><span data-stu-id="1d14c-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="1d14c-131">Để biết chi tiết, xem mục [Quy tắc giảm thiểu bề mặt tấn công](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="1d14c-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="1d14c-132">Xem lại các loại trừ đã áp dụng và xác minh dữ liệu sự kiện về lỗi chính sách hoặc ký tự đại diện bị hiểu sai.</span><span class="sxs-lookup"><span data-stu-id="1d14c-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="1d14c-133">Để biết thêm thông tin, hãy [xem Các loại loại trừ được hỗ trợ](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="1d14c-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="1d14c-134">nếu ảnh hưởng của quy tắc đó quá cao, hãy xem xét việc di chuyển quy tắc (quay lại) sang chế độ Kiểm tra để thực hiện xác thực thêm.</span><span class="sxs-lookup"><span data-stu-id="1d14c-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="1d14c-135">Để biết chi tiết, xem mục [Kiểm tra cách thức tính năng của Bộ bảo vệ Microsoft dành cho các tính năng Điểm cuối hoạt động trong chế độ kiểm tra](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="1d14c-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="1d14c-136">Thu thập dữ liệu hỗ trợ để mở trường hợp hỗ trợ bằng cách sử dụng lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="1d14c-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="1d14c-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="1d14c-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="1d14c-138">Để biết thêm thông tin, hãy [xem mục Sự cố với máy tích hợp cho Bộ bảo vệ Microsoft dành cho Điểm cuối.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="1d14c-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
