---
title: Bật các hộp thoại kế thừa nhúng để mở báo cáo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806457"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Bật các hộp thoại kế thừa nhúng để mở báo cáo

**Chứng**

Người dùng không thể mở báo cáo. "Có điều gì đó không ổn. Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "

**Bởi**

Báo cáo không tải trong UCI với lỗi, "bộ định dạng biểu mẫu là NULL hoặc không được xác định." Các báo cáo trong UCI vẫn yêu cầu các hộp thoại kế thừa, vì vậy hệ thống của khách hàng cần *phải có được* kích hoạt phân cấp bộ chọn.

**Nghiệm**

1. Đi đến **thiết đặt >quản trị > thiết đặt hệ thống > tab chung**.

2. Đặt "bật nhúng hộp thoại kế thừa nhất định trong máy khách trình duyệt giao diện hợp nhất" thành **có**.
