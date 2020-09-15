---
title: Tìm kiếm nội dung không có kết quả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680669"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="878d5-102">Không có kết quả nào từ tìm kiếm nội dung/xuất</span><span class="sxs-lookup"><span data-stu-id="878d5-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="878d5-103">Các sự cố với tìm kiếm nội dung/xuất không trả về bất kỳ dữ liệu nào có thể là do bộ lọc bảo mật nhất định được thiết lập bởi một người quản trị cụ thể và không liên lạc với tất cả người quản trị.</span><span class="sxs-lookup"><span data-stu-id="878d5-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="878d5-104">Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ bộ lọc bảo mật tuân thủ nào có thể gây ra điều này:</span><span class="sxs-lookup"><span data-stu-id="878d5-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="878d5-105">Kết nối với Trung tâm bảo mật và tuân thủ PowerShell</span><span class="sxs-lookup"><span data-stu-id="878d5-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="878d5-106">Chạy các commandlet sau đây:</span><span class="sxs-lookup"><span data-stu-id="878d5-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="878d5-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="878d5-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="878d5-108">Get-ComplianceSecurityFilter-tổ chức $org</span><span class="sxs-lookup"><span data-stu-id="878d5-108">Get-ComplianceSecurityFilter -Organization $org</span></span>