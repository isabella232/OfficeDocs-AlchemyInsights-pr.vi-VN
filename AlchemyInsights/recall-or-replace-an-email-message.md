---
title: Thu hồi hoặc thay thế thông điệp email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 2e711679e7db7293d9e7e6f68d0662f03047c23d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799226"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Thu hồi hoặc thay thế thông điệp email trong Microsoft 365

- Bạn chỉ có thể thu **hồi thư được gửi đến những người trong tổ chức của bạn**. Ví dụ: nếu thư đã được gửi đến một địa chỉ Gmail, chẳng hạn như bạn không thể thu hồi nó.
- Bạn chỉ có thể **gọi lại các thư được gửi từ Outlook 2016 cho PC**. Nếu người dùng gửi thư bằng cách dùng Outlook cho Mac hoặc Outlook trên web, bạn không thể thu hồi thư.
- Nếu bạn là người quản trị, bạn có thể thu **hồi thư thay mặt cho người dùng bằng cách sử dụng PowerShell**. Bạn không thể thu hồi thư từ Trung tâm quản trị. Cuộn xuống đến "tìm kiếm và xóa thông điệp email trong tổ chức của bạn" để biết thêm thông tin.

**Thu hồi hoặc thay thế thông điệp email mà bạn đã gửi**

1. Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục các mục đã gửi.
2. Mở thư mà bạn muốn thu hồi. Bạn phải bấm đúp để mở thư. Chọn thư để nó xuất hiện trong ngăn đọc sẽ không cho phép bạn thu hồi thư.
3. Từ tab thư, chọn **hành động**thu  >  **hồi thư này**.
4. Chọn **xóa bỏ các bản sao chưa đọc của thư này** hoặc **xóa bỏ các bản sao chưa đọc và thay thế bằng thư mới**, rồi chọn **OK**.
5. Nếu bạn đang gửi một thông báo thay thế, hãy soạn thư, rồi chọn **gửi**.
6. Sự thành công hay thất bại của thư được thu hồi tùy thuộc vào cài đặt của người nhận trong Outlook.

Để biết thêm thông tin, bao gồm cách kiểm tra việc thu hồi, hãy xem thu [hồi hoặc thay thế thông điệp email mà bạn đã gửi](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

***Tìm kiếm và xóa thông điệp email trong tổ chức của bạn*** Để tìm kiếm và xóa thông điệp email trong tổ chức của bạn, bạn nên dễ dàng nhất nếu bạn là người quản trị toàn cầu. Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào nhóm vai trò trình quản lý khám phá điện tử hoặc đối với vai trò quản lý tìm kiếm tuân thủ. Để xóa thư, bạn sẽ cần phải tham gia vào nhóm vai trò quản lý tổ chức hoặc vai trò tìm kiếm và dọn sạch quản lý. Quyền đối với các vai trò này được gán trong [Trung tâm tuân thủ & bảo mật](https://protection.office.com/).

1. [Tạo một tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/content-search) để tìm thư cần xóa.
2. [Kết nối với Trung tâm bảo mật & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps). 

Nếu bạn đang dùng MFA, hãy xem [kết nối với Microsoft 365 security & Trung tâm tuân thủ PowerShell bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps). 
