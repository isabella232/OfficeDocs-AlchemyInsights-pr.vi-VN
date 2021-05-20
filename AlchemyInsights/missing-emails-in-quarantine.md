---
title: Thiếu email trong cách ly
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539846"
---
# <a name="missing-emails-in-quarantine"></a>Thiếu email trong cách ly"

Người quản trị có [thể xem, phát hành hoặc xóa bỏ những thông báo này.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Để mở Trung tâm Bảo & Tuân thủ, hãy đi tới [https://protection.office.com](https://protection.office.com/) . Để mở trực tiếp trang Cách ly, hãy đi tới [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Bạn có thể tìm kiếm theo các giá trị sau:  

- **ID Thư:** Mã định danh duy nhất toàn cầu của thư. Nếu bạn chọn một thư trong danh sách, giá  **trị ID**  Thông báo sẽ xuất hiện  **trong**  ngăn cửa sổ bật lên Chi tiết xuất hiện. Người quản trị có thể dùng [công cụ tìm thư](/microsoft-365/security/office-365-security/message-trace-scc) để tìm thư và các giá trị ID Thư tương ứng của chúng.
- **Địa chỉ email người gửi:** Địa chỉ email của một người gửi đơn lẻ.
- **Địa chỉ email người** nhận: Địa chỉ email của một người nhận duy nhất.
- **Chủ** đề: Sử dụng toàn bộ chủ đề của thư. Tìm kiếm không có chữ hoa/thường.

Sau khi bạn đã nhập các tiêu chí tìm kiếm, hãy bấm ![ Làm mới nút ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Làm** mới để lọc kết quả.

Lệnh ghép ngắn mà bạn dùng để xem và quản lý thư và tệp trong cách ly là:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Lưu ý rằng lệnh ghép ngắn này chỉ dành cho thư, không phải tệp phần mềm xấu từ Bộ bảo vệ Microsoft cho Office 365 cho SharePoint Online, OneDrive for Business hoặc Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)