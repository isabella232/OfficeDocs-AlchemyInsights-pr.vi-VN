---
title: Khắc phục các ứng dụng Microsoft 365 không thể tìm thấy thư được liên kết với giấy phép Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747717"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Khắc phục các ứng dụng Microsoft 365 "không thể tìm thấy thông báo giấy phép Office được liên kết"

Nếu bạn nhận được thông báo này, hãy thử làm như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không chặn truy nhập Internet vào các ứng dụng Microsoft 365. Xem [URL và dải địa chỉ IP của Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Loại bỏ và [gán lại giấy phép Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) cho người dùng bị ảnh hưởng. 
3. Mở một ứng dụng Office và [đăng xuất khỏi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mọi tài khoản người dùng hiện có.
4. Đi đến thiết đặt Windows > **tài**khoản  >  **email & tài khoản**và loại bỏ tất cả tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.
5. Đi đến thiết đặt Windows > **tài khoản**  >  **Access hoặc trường học**và ngắt kết nối tất cả các tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.
6. Đặt lại trạng thái kích hoạt Office. [Tìm hiểu cách thức](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Đăng nhập](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.

Để biết các giải pháp khắc phục sự cố bổ sung, hãy xem các [lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).