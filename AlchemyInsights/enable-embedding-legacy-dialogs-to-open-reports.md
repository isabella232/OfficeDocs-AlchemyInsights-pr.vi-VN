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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003411"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Bật các hộp thoại kế thừa nhúng để mở báo cáo

**Dấu hiệu**

Người dùng không thể mở báo cáo. "Đã xảy ra sự cố. Hãy kiểm tra các chi tiết kỹ thuật để biết thêm chi tiết".

**Nguyên nhân**

Báo cáo không tải được ở UCI kèm theo lỗi "Biểu mẫu mô tả là null hoặc không được xác định." Báo cáo trong UCI vẫn yêu cầu các hộp thoại thừa tự, vì vậy hệ thống của khách hàng cần được bật *allowlegacydialogsembedding.*

**Giải pháp**

1. Đi đến **tab Cài đặt >Quản > Hệ Cài đặt > Chung.**

2. Đặt "Bật nhúng của một số hộp thoại thừa tự nhất định trong máy khách trình duyệt Giao diện Hợp nhất" **thành Có.**
