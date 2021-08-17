---
title: Công cụ Khám phá Điện tử Thừa tự
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
- "9001487"
- "3523"
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074702"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Công cụ Khám phá Điện tử Thừa tự

Do chức năng Khám phá Điện tử mới và được cải thiện trong Trung tâm Tuân thủ Microsoft 365, các công cụ và lệnh lệnh Khám phá Điện tử kế thừa sau đây sẽ bị ngừng sử dụng trong những tháng sắp tới:

- [Khám phá Điện tử Tại chỗ và](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) Giữ Tại Chỗ [trong](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) trung tâm quản Exchange chính.

- Lệnh ghép Exchange Online PowerShell hỗ trợ In-Place khám phá Điện tử In-Place giữ. (Các lệnh ghép ngắn này được xác định chung là *-MailboxSearch lệnh ghép ngắn.) Bao gồm các lệnh ghép ngắn sau:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Lệnh [ghép ngắn Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) trong Exchange Online PowerShell.
- Các thao tác sau đây trong EXCHANGE Web Services API:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Đường thời gian để nghỉ hưu:**
- **01/07/2020** Bạn không còn có thể tạo tìm kiếm và giữ mới, nhưng bạn có thể chạy, sửa và xóa các tìm kiếm hiện có với mọi rủi ro do bạn tự rủi ro. Hỗ trợ của Microsoft không còn hỗ In-Place Giữ Nội & Khám phá Điện tử trong EAC.
    
- Ngày 1 tháng **10 năm 2020,** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.

**Để biết thêm thông tin, hãy xem:**

 - [Di chuyển các tìm kiếm và giữ Lại Khám phá Điện tử thừa tự vào thư Trung tâm tuân thủ Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Các công cụ Khám phá Điện tử kế thừa](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Câu hỏi thường gặp In-Place khám phá Điện tử và In-Place Giữ](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



