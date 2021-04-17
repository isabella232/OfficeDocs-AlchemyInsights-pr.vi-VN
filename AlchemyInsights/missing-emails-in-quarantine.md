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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831756"
---
# <a name="missing-emails-in-quarantine"></a>Thiếu email trong cách ly "

Người quản trị có thể [xem, phát hành hoặc xóa các thư này.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Để mở Trung tâm tuân thủ & bảo mật, hãy đi tới [https://protection.office.com](https://protection.office.com/) . Để mở trực tiếp trang cách ly, hãy đi đến [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Bạn có thể tìm kiếm theo các giá trị sau:  

- **ID thông báo: mã** định danh duy nhất trên toàn cầu của thư. Nếu bạn chọn một thư trong danh sách, giá trị  **ID thông báo**  sẽ xuất hiện trong ngăn  **thông tin chi tiết**  xuất hiện. Người quản trị có thể sử dụng theo [dõi thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) để tìm thư và các giá trị ID thông báo tương ứng của chúng.
- **Địa chỉ email người gửi**: địa chỉ email của một người gửi.
- **Địa chỉ email người nhận**: địa chỉ email của một người nhận.
- **Subject**: dùng toàn bộ chủ đề của thư. Tìm kiếm không phân biệt chữ hoa/thường.

Sau khi bạn đã nhập tiêu chí tìm kiếm, bấm làm mới nút làm mới ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  để lọc kết quả.  

Các lệnh ghép ngắn mà bạn sử dụng để xem và quản lý các thư và tệp trong cách ly:
- [Xóa-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- Bản [xem trước-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): lưu ý rằng lệnh ghép ngắn này chỉ dành cho các thư, không phải tệp phần mềm độc hại từ ATP cho SharePoint Online, OneDrive for Business hoặc nhóm.
- [Bản phát hành-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)