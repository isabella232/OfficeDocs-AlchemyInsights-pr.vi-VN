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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516801"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="3b77f-102">Không có kết quả từ nội dung tìm kiếm/xuất khẩu</span><span class="sxs-lookup"><span data-stu-id="3b77f-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="3b77f-103">Vấn đề với nội dung tìm kiếm/xuất khẩu không trả lại bất kỳ dữ liệu có thể là do một số bộ lọc bảo mật tuân thủ đã là thiết lập bởi một quản trị viên cụ thể và không giao tiếp với tất cả các quản trị viên.</span><span class="sxs-lookup"><span data-stu-id="3b77f-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="3b77f-104">Để giải quyết điều này, hãy kiểm tra xem nếu có bất kỳ bộ lọc bảo mật tuân thủ có thể gây ra điều này:</span><span class="sxs-lookup"><span data-stu-id="3b77f-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="3b77f-105">Kết nối bảo mật và tuân thủ trung tâm Powershell</span><span class="sxs-lookup"><span data-stu-id="3b77f-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="3b77f-106">Chạy commandlets sau đây:</span><span class="sxs-lookup"><span data-stu-id="3b77f-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="3b77f-107">$org = "Tenmiencuaban.com"</span><span class="sxs-lookup"><span data-stu-id="3b77f-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="3b77f-108">Get-ComplianceSecurityFilter-tổ chức $org</span><span class="sxs-lookup"><span data-stu-id="3b77f-108">Get-ComplianceSecurityFilter -Organization $org</span></span>