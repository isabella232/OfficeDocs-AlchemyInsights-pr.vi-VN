---
title: Ví dụ về Bộ bảo vệ Microsoft Office 365 sách chống lừa đảo qua web
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035028"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Ví dụ về Bộ bảo vệ Microsoft Office 365 sách chống lừa đảo qua web

Những thiết đặt này kích hoạt một chính sách gọi *là Tên miền và Tổng Giám đốc*. Chính sách này cung cấp cả bảo vệ người dùng và tên miền khỏi mạo danh và sau đó áp dụng chính sách cho tất cả email mà người dùng trong miền nhận được. Trước tiên, hãy thêm các thông tin sau đây để tạo chính sách:

- **Tên**: Mô tả Tên miền **và Giám** đốc Điều hành : Đảm bảo rằng Tổng Giám Đốc và tên miền của bạn không bị mạo danh.
  **Áp dụng cho:** Chọn **miền người nhận là**. Bên **dưới bất kỳ dịch vụ** nào trong số **này, chọn** Chọn , rồi chọn một miền. Chọn **+ Thêm**. Chọn hộp kiểm cạnh tên miền trong danh sách (ví dụ: tên miền *contoso.com*), sau đó chọn **Thêm**. Chọn **Xong**.
- Sau khi chính sách được tạo, bạn có thể tinh chỉnh chính sách bằng cách sử dụng các tùy chọn sau đây:
  - **Thêm người dùng để bảo vệ:** Ví dụ: thêm địa chỉ email của Tổng Giám đốc ở mức tối thiểu.
  - **Thêm miền để bảo vệ:** Thêm miền tổ chức có chứa văn phòng Tổng Giám đốc.
  - **Chọn hành** động : Đối với Nếu email được gửi bởi người dùng mạo danh, hãy chọn Chuyển hướng thư đến địa chỉ **email** khác , rồi nhập địa chỉ **email** của người quản trị bảo mật (ví dụ: *securityadmin@contoso.com).* Đối **với Nếu email được gửi bởi một tên miền mạo danh,** chọn **Cách ly thư**.
  - **Thông minh** hộp thư : Theo mặc định, tùy chọn này được chọn khi bạn tạo một chính sách chống lừa đảo mới. Để cài đặt này **là Bật để** có kết quả tốt nhất.
  - **Thêm người gửi và tên miền tin cậy:** Ví dụ: không xác định bất kỳ ghi đè nào.
- Sau khi đã xem lại cài đặt của mình, chọn **Tạo chính sách này hoặc** **Lưu**, tùy trường hợp.

Để tìm hiểu thêm, hãy [xem chính sách Chống lừa đảo qua Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
