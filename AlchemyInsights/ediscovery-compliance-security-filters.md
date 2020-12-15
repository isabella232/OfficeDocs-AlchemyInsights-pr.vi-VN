---
title: Không có kết quả nào được trả về khi tìm kiếm nội dung/xuất
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680333"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="12e5c-102">Không có kết quả nào được trả về khi tìm kiếm nội dung/xuất</span><span class="sxs-lookup"><span data-stu-id="12e5c-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="12e5c-103">Nếu bạn đang gặp vấn đề với các kịch bản khám phá điện tử sau đây:</span><span class="sxs-lookup"><span data-stu-id="12e5c-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="12e5c-104">Tìm kiếm nội dung/xuất không trả về dữ liệu hoặc dữ liệu không mong muốn</span><span class="sxs-lookup"><span data-stu-id="12e5c-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="12e5c-105">Tìm kiếm khám phá điện tử hoặc xuất không thành công</span><span class="sxs-lookup"><span data-stu-id="12e5c-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="12e5c-106">Điều này có thể gây ra do một số bộ lọc bảo mật tuân thủ nhất định được thiết lập bởi một người quản trị cụ thể và không được truyền đạt đến tất cả người quản trị.</span><span class="sxs-lookup"><span data-stu-id="12e5c-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="12e5c-107">Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ bộ lọc bảo mật tuân thủ nào có thể gây ra sự cố này không:</span><span class="sxs-lookup"><span data-stu-id="12e5c-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="12e5c-108">Kết nối với Trung tâm bảo mật và tuân thủ PowerShell</span><span class="sxs-lookup"><span data-stu-id="12e5c-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="12e5c-109">Chạy các commandlet sau đây:</span><span class="sxs-lookup"><span data-stu-id="12e5c-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="12e5c-110">Để biết thêm thông tin về bộ lọc bảo mật tuân thủ, hãy xem [lọc quyền đối với tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="12e5c-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
