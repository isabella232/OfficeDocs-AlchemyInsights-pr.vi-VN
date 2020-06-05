---
title: Thiếu email trong cách ly
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569565"
---
# <a name="missing-emails-in-quarantine"></a>Thiếu email trong kiểm dịch "

Quản trị viên có thể [xem, phát hành hoặc xoá các thư này.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Để mở Trung tâm tuân thủ & bảo mật, hãy chuyển đến [https://protection.office.com](https://protection.office.com/) . Để mở trực tiếp trang cách ly, hãy chuyển đến [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Bạn có thể tìm kiếm theo các giá trị sau:  

- **Message ID**: mã định danh duy nhất toàn cầu của thư. Nếu bạn chọn một thư trong danh sách, giá trị **ID thư** sẽ xuất hiện trong ngăn hộp thả xuống **chi tiết** xuất hiện. Quản trị viên có thể sử dụng [theo dõi thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) để tìm thư và các giá trị Message ID tương ứng.
- **Địa chỉ email người gửi**: một địa chỉ email của người gửi duy nhất.
- **Địa chỉ email người nhận**: địa chỉ email của một người nhận.
- **Chủ**đề: sử dụng toàn bộ chủ đề của tin nhắn. Tìm kiếm không phải là chữ.

Sau khi bạn đã nhập tiêu chí tìm kiếm, hãy nhấp vào Refresh ![ nút ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** để lọc kết quả.  

Các lệnh ghép ngắn bạn sử dụng để xem và quản lý thư và tệp cách ly là:
- [Xóa-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Xuất-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Xem trước-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): lưu ý rằng lệnh này chỉ dành cho các thư, không phải tệp phần mềm độc hại từ ATP cho SharePoint Online, OneDrive for Business hoặc teams.
- [Phát hành-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)