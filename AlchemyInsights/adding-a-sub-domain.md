---
title: Thêm miền con
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506765"
---
# <a name="adding-a-sub-domain"></a>Thêm miền con

Miền con có thể được thêm vào cùng một đối tượng thuê hoặc đối tượng thuê khác với miền mẹ. Trong cả hai trường hợp, bạn phải quản lý thiết đặt DNS của riêng mình tại website của nhà đăng ký. Nếu bạn đã cho phép Microsoft quản lý thiết đặt DNS của bạn với bản ghi NS, hoặc nếu bạn đã mua tên miền từ Microsoft, bạn không thể thêm tên miền con mà không thay đổi điều này trước tiên.

Thêm tên miền mẹ trước, sau đó thêm tên miền con. Nếu tên miền con nằm trong cùng một đối tượng thuê, không cần xác nhận bổ sung. Nếu thêm miền con vào một đối tượng thuê riêng, cần có bản ghi txt DNS để xác minh quyền sở hữu trước khi thêm miền và các bản ghi DNS bổ sung cho các dịch vụ đã chọn.

- Để thêm miền hoặc tên miền [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)con, hãy làm theo trình hướng dẫn Thêm Miền hoặc thêm miền hoặc tên miền con theo cách thủ công bằng cách vào Thiết đặt Miền  >    >  **Thêm miền.**

Nếu cần thiết:

- Để thay đổi người quản lý thiết đặt DNS của bạn cho tên miền hiện có, hãy đi tới **Cài đặt**  >  [**Domains**](https://admin.microsoft.com/Adminportal/Home#/Domains), chọn hộp kiểm bên cạnh tên miền, sau đó chọn Quản lý **DNS**. Trong trình hướng dẫn, chọn Thêm **bản ghi DNS của riêng bạn, rồi** hoàn tất trình hướng dẫn.
- Để thêm tên miền con vào miền microsoft đã mua, trước tiên hãy chuyển tên miền đó cho một nhà đăng ký khác, sau đó thực hiện thay đổi ở trên để quản lý bản ghi DNS của riêng bạn. Để biết hướng dẫn, [xem mục Chuyển miền từ Microsoft sang một máy chủ khác.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Nếu bạn nhận được lỗi rằng tên miền của bạn đã được các thành viên khác hoặc những người trong tổ chức của bạn sử dụng, trước tiên bạn sẽ cần kiểm soát tài khoản không được quản lý này trước khi sử dụng tên miền. Để biết hướng dẫn, hãy [xem Tiếp quản thư mục không được quản lý với tư cách người quản trị Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
