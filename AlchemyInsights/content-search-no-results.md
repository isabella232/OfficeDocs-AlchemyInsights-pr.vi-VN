---
title: Nội dung tìm kiếm không có kết quả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800698"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="bf155-102">Không có kết quả từ nội dung tìm kiếm/xuất khẩu</span><span class="sxs-lookup"><span data-stu-id="bf155-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="bf155-103">Vấn đề với nội dung tìm kiếm/xuất khẩu không trả lại bất kỳ dữ liệu có thể là do một số bộ lọc bảo mật tuân thủ đã là thiết lập bởi một quản trị viên cụ thể và không giao tiếp với tất cả các quản trị viên.</span><span class="sxs-lookup"><span data-stu-id="bf155-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="bf155-104">Để giải quyết điều này, hãy kiểm tra xem nếu có bất kỳ bộ lọc bảo mật tuân thủ có thể gây ra điều này:</span><span class="sxs-lookup"><span data-stu-id="bf155-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="bf155-105">Kết nối bảo mật và tuân thủ trung tâm Powershell</span><span class="sxs-lookup"><span data-stu-id="bf155-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="bf155-106">Chạy commandlets sau đây:</span><span class="sxs-lookup"><span data-stu-id="bf155-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="bf155-107">$org = "Tenmiencuaban.com"</span><span class="sxs-lookup"><span data-stu-id="bf155-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="bf155-108">Get-ComplianceSecurityFilter-tổ chức $org</span><span class="sxs-lookup"><span data-stu-id="bf155-108">Get-ComplianceSecurityFilter -Organization $org</span></span>