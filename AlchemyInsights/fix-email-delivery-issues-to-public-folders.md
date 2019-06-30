---
title: Sửa chữa các vấn đề phân phối email để kích hoạt thư thư mục công cộng
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387727"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Sửa chữa các vấn đề phân phối email để kích hoạt thư thư mục công cộng

Nếu người gửi bên ngoài không thể gửi thư đến thư mục công cộng của bạn kích hoạt thư, và những người gửi nhận được lỗi: **không thể được tìm thấy (550 5.4.1)**, xác minh tên miền thư điện tử cho thư mục chung được đặt cấu hình làm miền chuyển tiếp nội bộ thay vì một miền uỷ quyền:

1. Mở [Trung tâm quản trị Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Đi đến **luồng thư** \> **tên miền được chấp nhận**, hãy chọn các tên miền được chấp nhận, và sau đó nhấp vào **chỉnh sửa**.

3. Trong các thuộc tính trang đó sẽ mở ra, nếu loại miền được thiết lập để **Authoritative**, thay đổi giá trị thành **chuyển tiếp nội bộ** và sau đó nhấp vào **lưu**.

Nếu người gửi bên ngoài nhận được lỗi **bạn không có quyền (550 5.7.13)**, hãy chạy lệnh sau trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem các quyền cho người dùng vô danh trong thư mục công cộng:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ví dụ, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

Để cho phép người dùng bên ngoài gửi email đến thư mục chung, hãy thêm truy cập CreateItems ngay cho người dùng chưa xác định người. Ví dụ, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
