---
title: Bật các hộp thoại kế thừa nhúng để mở báo cáo
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814286"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Bật các hộp thoại kế thừa nhúng để mở báo cáo

**Chứng**

Người dùng không thể mở báo cáo. "Có điều gì đó không ổn. Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "

**Bởi**

Báo cáo không tải trong UCI với lỗi, "bộ định dạng biểu mẫu là NULL hoặc không được xác định." Các báo cáo trong UCI vẫn yêu cầu các hộp thoại kế thừa, vì vậy hệ thống của khách hàng cần *phải có được* kích hoạt phân cấp bộ chọn.

**Nghiệm**

1. Đi đến **thiết đặt >quản trị > thiết đặt hệ thống > tab chung**.

2. Đặt "bật nhúng hộp thoại kế thừa nhất định trong máy khách trình duyệt giao diện hợp nhất" thành **có**.
