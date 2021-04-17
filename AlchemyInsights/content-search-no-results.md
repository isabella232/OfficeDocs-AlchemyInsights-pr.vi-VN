---
title: Tìm kiếm nội dung không có kết quả
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816870"
---
# <a name="no-results-from-content-searchexports"></a>Không có kết quả nào từ tìm kiếm nội dung/xuất

Các sự cố với tìm kiếm nội dung/xuất không trả về bất kỳ dữ liệu nào có thể là do bộ lọc bảo mật nhất định được thiết lập bởi một người quản trị cụ thể và không liên lạc với tất cả người quản trị.

Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ bộ lọc bảo mật tuân thủ nào có thể gây ra điều này:
1. Kết nối với Trung tâm bảo mật và tuân thủ PowerShell
2. Chạy các commandlet sau đây:
<br>$org = "yourdomain.com"
<br>$Org Get-ComplianceSecurityFilter tổ chức