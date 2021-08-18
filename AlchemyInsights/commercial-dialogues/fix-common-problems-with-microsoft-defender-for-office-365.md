---
title: Khắc phục các sự cố phổ biến với Bộ bảo vệ Microsoft dành cho Office 365
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
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330082"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Khắc phục các sự cố phổ biến với Bộ bảo vệ Microsoft dành cho Office 365

Dưới đây là một số giải pháp cho các sự cố phổ biến với Bộ bảo vệ Microsoft dành cho Office 365:

- **Độ trễ thư:**

  Sự chậm trễ trong việc chuyển phát email có thể là Két sắt đến việc quét tệp đính kèm của thư. Để biết thêm thông tin, hãy [xem Két sắt chính sách Phần đính kèm.](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings)

- **Báo cáo kết quả dương hoặc âm báo cáo sai:**

  Để biết thêm thông tin, hãy [xem mục Báo cáo thư và tệp cho Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Bật Bảo Két sắt nối kết:**

  1. Trong cổng thông tin Bộ bảo vệ Microsoft 365 , đi đến Chính sách Cộng tác qua Email & & chính sách Mối đe dọa trong Quy Két sắt Nối kết trong <https://security.microsoft.com/>  \>  \>  \>  **phần Chính** sách.

     Để đi thẳng tới trang **Liên Két sắt,** hãy sử dụng <https://security.microsoft.com/safelinksv2> .

  2. Trên trang **Két sắt Liên kết,** hãy chọn chính sách bằng cách bấm vào tên của chính sách.
  3. Trong phần bật lên chi tiết xuất hiện, hãy thực hiện một trong các bước sau đây:
     - Để thêm chính sách mới, chọn **+ Tạo**. Một trình hướng dẫn sẽ khởi chạy để giúp bạn xác định các thiết đặt chính sách.
     - Để sửa chính sách hiện có, hãy chọn chính sách bằng cách bấm vào tên của chính sách. Trong hộp bật lên chi tiết xuất hiện, chọn Chỉnh **sửa trong** mục Cài **đặt bảo** vệ.
  4. Trên trang Thiết **đặt bảo vệ,** cấu hình các thiết đặt sau:
     - Bật Chọn hành **động cho URL độc hại tiềm ẩn không xác định trong thư.**
     - Chọn Áp **dụng các liên kết an toàn cho các tin nhắn đã gửi trong tổ chức**.

  Để biết thêm thông tin, xem [mục Thiết lập liên Két sắt chính sách Liên kết trong Bộ bảo vệ Microsoft cho Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
