---
title: Outlook Desktop thu hồi hoặc thay thế thông điệp email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664012"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>Thu hồi hoặc thay thế thông điệp email Outlook

- Với tư cách là người quản trị, bạn có thể thu **hồi thư thay mặt cho người dùng bằng PowerShell**. Bạn không thể thu hồi thư từ Trung tâm quản trị.
- Bạn chỉ có thể thu **hồi thư được gửi đến những người trong tổ chức của bạn**. Ví dụ: nếu thư đã được gửi đến một địa chỉ Gmail, chẳng hạn như bạn không thể thu hồi nó.
- Bạn chỉ có thể **gọi lại các thư được gửi từ Outlook 2016 trên PC**. Nếu người dùng gửi thư bằng cách dùng Outlook cho Mac hoặc Outlook trên web, bạn không thể thu hồi thư.

Để thu hồi hoặc thay thế thông điệp email:

1. Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục các mục đã gửi.
1. Bấm đúp vào thư mà bạn muốn thu hồi để mở.
1. Chọn tab **thư** , rồi chọn **hành động**thu  >  **hồi thư này**.
1. Chọn **xóa bỏ các bản sao chưa đọc của thư này** hoặc **xóa bỏ các bản sao chưa đọc và thay thế bằng thư mới**, rồi chọn **OK**.
1. Nếu bạn đang gửi một thông báo thay thế, soạn thư, rồi chọn **gửi**.
1. Sự thành công hoặc thất bại của thư được thu hồi tùy thuộc vào cài đặt của người nhận trong Outlook. Để biết các bước kiểm tra lại, hãy xem [bài viết này](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

Tìm kiếm và xóa thông điệp email trong tổ chức của bạn

- Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào vai trò quản lý khám phá điện tử hoặc vai trò tìm kiếm tuân thủ để tìm kiếm thư. Để xóa thư, bạn sẽ cần phải tham gia vào nhóm vai trò quản lý tổ chức hoặc vai trò tìm kiếm và dọn sạch quản lý. Quyền cho các vai trò này được gán trong [Trung tâm bảo mật và tuân thủ](https://go.microsoft.com/fwlink/?linkid=2083731).
- [Tạo một tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/content-search) để tìm thư cần xóa.
- [Kết nối với Trung tâm bảo mật và tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).

Nếu bạn đang sử dụng xác thực đa yếu tố, hãy xem [kết nối với Trung tâm bảo mật và tuân thủ Microsoft 365 bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).