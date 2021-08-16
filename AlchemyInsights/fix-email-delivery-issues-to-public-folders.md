---
title: Khắc phục sự cố chuyển phát email đối với thư mục công cộng hỗ trợ thư
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ff1400f694ae037a8658356af068b4c20b8fa9d9908dafedb90db7bb6859530f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068834"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Khắc phục sự cố chuyển phát email đối với thư mục công cộng hỗ trợ thư

Nếu người gửi bên ngoài không thể gửi thư đến thư mục công cộng hỗ trợ thư của bạn và người gửi sẽ nhận được lỗi: không thể tìm thấy : không thể tìm thấy **(550 5.4.1),** hãy xác minh miền email cho thư mục công cộng được cấu hình dưới dạng một miền chuyển tiếp nội bộ thay vì một tên miền có thẩm quyền:

1. Mở Trung [Exchange quản trị Viên Hệ thống (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. Đi tới Dòng **thư Tên** miền được \> **chấp nhận**, chọn tên miền được chấp nhận, rồi bấm **Sửa.**

3. Trong trang thuộc tính mở ra, nếu loại tên miền được đặt là Có thẩm **quyền,** hãy thay đổi giá trị thành **Chuyển** tiếp bên trong và sau đó bấm **Lưu.**

Nếu người gửi bên ngoài nhận được lỗi mà bạn không có quyền **(550 5.7.13),** hãy chạy lệnh sau trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem các quyền cho người dùng ẩn danh trong thư mục công cộng:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Ví dụ, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Để cho phép người dùng bên ngoài gửi email đến thư mục công cộng này, hãy thêm quyền truy nhập CreateItems ngay vào người dùng Ẩn danh. Ví dụ, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .
