---
title: Không trả về kết quả trong quá trình Tìm kiếm/Xuất Nội dung
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101288"
---
# <a name="no-results-returned-during-content-searchexport"></a>Không trả về kết quả trong quá trình Tìm kiếm/Xuất Nội dung

Nếu bạn đang gặp phải sự cố với các kịch bản Khám phá Điện tử sau đây:

- Tìm kiếm Nội dung/Xuất không trả về dữ liệu hoặc dữ liệu không mong muốn
- Tìm kiếm hoặc Xuất Khám phá Điện tử không thành công

Điều này có thể do một số Bộ lọc Bảo mật Tuân thủ nhất định đã được một Người quản trị cụ thể thiết lập và chưa được thông báo cho tất cả người quản trị.

Để giải quyết vấn đề này, hãy kiểm tra xem có bất kỳ Bộ lọc Bảo mật Tuân thủ nào có thể gây ra những vấn đề này không:

1. Kết nối powershell của Trung tâm Bảo mật và Tuân thủ
2. Chạy lệnh dưới đây:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Để biết thêm thông tin về Bộ lọc Bảo mật Tuân thủ, [hãy xem Lọc Quyền cho Tìm kiếm Nội dung](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
