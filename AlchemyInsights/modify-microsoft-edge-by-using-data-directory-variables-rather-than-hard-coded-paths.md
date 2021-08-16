---
title: Sửa đổi Microsoft Edge dùng biến thư mục dữ liệu thay vì đường dẫn được mã hóa cố định
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992313"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Sửa đổi Microsoft Edge dùng biến thư mục dữ liệu thay vì đường dẫn được mã hóa cố định

Ví dụ: trên Windows, để lưu trữ dữ liệu hồ sơ dưới dữ liệu ứng dụng cục bộ của người dùng thay vì tại vị trí mặc định, hãy đặt chính sách *UserDataDir* **thành ${local_app_data}\Edge\Profile**.

Để biết thêm thông tin, [hãy xem Tạo Microsoft Edge thư mục dữ liệu người dùng](https://docs.microsoft.com/deployedge/microsoft-edge-policies).