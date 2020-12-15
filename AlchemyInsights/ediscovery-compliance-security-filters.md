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
# <a name="no-results-returned-during-content-searchexport"></a>Không có kết quả nào được trả về khi tìm kiếm nội dung/xuất

Nếu bạn đang gặp vấn đề với các kịch bản khám phá điện tử sau đây:

- Tìm kiếm nội dung/xuất không trả về dữ liệu hoặc dữ liệu không mong muốn
- Tìm kiếm khám phá điện tử hoặc xuất không thành công

Điều này có thể gây ra do một số bộ lọc bảo mật tuân thủ nhất định được thiết lập bởi một người quản trị cụ thể và không được truyền đạt đến tất cả người quản trị.

Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ bộ lọc bảo mật tuân thủ nào có thể gây ra sự cố này không:

1. Kết nối với Trung tâm bảo mật và tuân thủ PowerShell
2. Chạy các commandlet sau đây:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Để biết thêm thông tin về bộ lọc bảo mật tuân thủ, hãy xem [lọc quyền đối với tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
