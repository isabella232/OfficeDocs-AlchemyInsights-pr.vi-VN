---
title: Sửa đổi Microsoft Edge bằng cách dùng các biến dữ liệu của thư mục thay vì đường dẫn mã cứng
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
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036862"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Sửa đổi Microsoft Edge bằng cách dùng các biến dữ liệu của thư mục thay vì đường dẫn mã cứng

Ví dụ, trên Windows, để lưu trữ dữ liệu hồ sơ dưới dữ liệu ứng dụng cục bộ của người dùng thay vì ở vị trí mặc định, hãy đặt chính sách *Userdatadir* thành **$ {local_app_data} \Edge\Profile**.

Để biết thêm thông tin, hãy xem [tạo các biến số thư mục dữ liệu người dùng Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).