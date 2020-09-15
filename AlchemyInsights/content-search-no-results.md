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
# <a name="no-results-from-content-searchexports"></a>Không có kết quả nào từ tìm kiếm nội dung/xuất

Các sự cố với tìm kiếm nội dung/xuất không trả về bất kỳ dữ liệu nào có thể là do bộ lọc bảo mật nhất định được thiết lập bởi một người quản trị cụ thể và không liên lạc với tất cả người quản trị.

Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ bộ lọc bảo mật tuân thủ nào có thể gây ra điều này:
1. Kết nối với Trung tâm bảo mật và tuân thủ PowerShell
2. Chạy các commandlet sau đây:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-tổ chức $org