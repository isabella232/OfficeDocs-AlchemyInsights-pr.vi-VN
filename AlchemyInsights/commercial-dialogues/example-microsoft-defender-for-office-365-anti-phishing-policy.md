---
title: Ví dụ về Microsoft Defender cho chính sách chống lừa đảo qua Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751116"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Ví dụ về Microsoft Defender cho chính sách chống lừa đảo qua Office 365

Các thiết đặt này cho phép một chính sách có tên là *Domain và CEO*. Chính sách này cung cấp cho cả người dùng và bảo vệ tên miền khỏi mạo danh và sau đó áp dụng chính sách cho tất cả người dùng nhận được email bên trong tên miền. Trước tiên, hãy thêm thông tin sau đây để tạo chính sách:

- **Tên**: Domain và CEO **mô tả**: đảm bảo rằng giám đốc điều hành và tên miền của bạn đang không bị mạo danh.
  Được **áp dụng cho**: chọn **tên miền của người nhận**. Bên dưới **bất kỳ phần nào trong số này**, hãy chọn **chọn**, rồi chọn tên miền. Chọn **+ Thêm**. Chọn hộp kiểm bên cạnh tên miền trong danh sách (ví dụ, *contoso.com*), rồi chọn **Thêm**. Chọn đã **xong**.
- Sau khi chính sách được tạo ra, bạn có thể tinh chỉnh chính sách bằng cách sử dụng các tùy chọn sau đây:
  - **Thêm người dùng để bảo vệ:** Đối với ví dụ này, hãy thêm địa chỉ email của giám đốc điều hành, ở mức tối thiểu.
  - **Thêm tên miền để bảo vệ**: thêm tên miền tổ chức bao gồm Office của giám đốc điều hành.
  - **Chọn hành động**: **nếu email được gửi bởi người dùng mạo** danh, hãy chọn **chuyển hướng thư đến một địa chỉ email khác**, sau đó nhập địa chỉ email của người quản trị bảo mật (ví dụ, *securityadmin@contoso.com*). **Nếu email được gửi bởi tên miền mạo** danh, hãy chọn cách **ly thư**.
  - **Thông minh trong hộp thư**: theo mặc định, tùy chọn này được chọn khi bạn tạo chính sách chống lừa đảo qua mạng mới. Rời khỏi thiết đặt này để có kết quả **tốt nhất.**
  - **Thêm người gửi và tên miền đáng tin cậy:** Đối với ví dụ này, không xác định ghi đè.
- Sau khi bạn đã xem lại các thiết đặt của mình, hãy chọn **tạo chính sách này** hoặc **lưu**, như phù hợp.

Để tìm hiểu thêm, hãy xem [chính sách chống lừa đảo trong Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
