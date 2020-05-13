---
title: Cho phép nhúng hộp thoại kế thừa để mở báo cáo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204681"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Cho phép nhúng hộp thoại kế thừa để mở báo cáo

**Triệu chứng**

Người dùng không thể mở báo cáo. "Cái gì đã đi sai. Kiểm tra chi tiết kỹ thuật để biết thêm chi tiết. "

**Gây ra**

Báo cáo không tải UCI với lỗi "mô tả mẫu là NULL hoặc không xác định." Báo cáo trong UCI vẫn yêu cầu hộp thoại kế thừa, do đó, Hệ thống của khách hàng cần phải có *allowlegacydialogsembedding* kích hoạt.

**Giải pháp**

1. Đi tới **cài đặt >quản trị > thiết đặt hệ thống > tab chung**.

2. Đặt "bật nhúng các hộp thoại kế thừa nhất định trong ứng dụng trình duyệt giao diện hợp nhất" thành **có**.
