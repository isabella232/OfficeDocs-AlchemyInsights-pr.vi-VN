---
title: Sửa chữa Microsoft 365 ứng dụng không thể tìm thấy giấy phép văn phòng liên quan đến tin nhắn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580463"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Khắc phục thông báo Microsoft 365 ứng dụng "không thể tìm thấy giấy phép Office liên kết"

Nếu bạn nhận được thông báo này, hãy thử như sau:

1. Kiểm tra tường lửa, phần mềm chống vi-rút và cài đặt proxy để xác nhận rằng chúng không chặn truy cập Internet tới các ứng dụng Microsoft 365. Xem [Microsoft 365 URL và phạm vi địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Loại bỏ và [gán giấy phép Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) cho người dùng bị ảnh hưởng. 
3. Mở ứng dụng Office và [đăng](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) xuất khỏi bất kỳ tài khoản người dùng hiện có nào.
4. Đi tới cài đặt Windows > **tài**khoản  >  **email & tài khoản**và xóa tất cả tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.
5. Đi tới cài đặt Windows > **tài khoản**  >  **truy cập làm việc hoặc trường**và ngắt kết nối tất cả các tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.
6. Đặt lại trạng thái kích hoạt Office. [Tìm hiểu làm thế nào](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Đăng nhập](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.

Để biết thêm giải pháp khắc phục sự cố, xem các [lỗi kích hoạt và sản phẩm không được cấp phép trong Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).