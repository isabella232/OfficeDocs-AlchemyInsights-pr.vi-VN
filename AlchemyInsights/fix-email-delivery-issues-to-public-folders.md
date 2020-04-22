---
title: Khắc phục sự cố gửi email cho thư mục công cộng kích hoạt thư
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716374"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Khắc phục sự cố gửi email cho thư mục công cộng kích hoạt thư

Nếu người gửi bên ngoài không thể gửi thư đến thư mục công cộng kích hoạt thư của bạn, và các bên gửi nhận được lỗi: **không thể tìm thấy (550 5.4.1)**, kiểm tra miền email cho thư mục công cộng được cấu hình là một miền chuyển tiếp nội bộ thay vì một miền uỷ quyền:

1. Mở [Trung tâm quản trị Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Đi tới \> **miền được chấp nhận** **dòng thư** , chọn miền chấp nhận, sau đó bấm vào **chỉnh sửa**.

3. Trong trang thuộc tính mở ra, nếu loại miền được đặt thành **uỷ**quyền, thay đổi giá trị chuyển **tiếp nội bộ** và sau đó bấm **lưu**.

Nếu người gửi bên ngoài nhận được lỗi **bạn không có quyền (550 5.7.13)**, hãy chạy lệnh sau trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem quyền ẩn danh trong thư mục công cộng:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ví dụ: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Để cho phép người dùng bên ngoài gửi email đến thư mục công cộng này, thêm truy cập CreateItems quyền người dùng ẩn danh. Ví dụ: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
