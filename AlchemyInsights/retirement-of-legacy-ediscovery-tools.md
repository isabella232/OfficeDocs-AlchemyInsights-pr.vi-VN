---
title: Nghỉ hưu của Legacy eDiscovery công cụ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157764"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Nghỉ hưu của Legacy eDiscovery công cụ

Là kết quả mới và cải tiến eDiscovery chức năng trong Microsoft 365 Trung tâm tuân thủ, hợp lệ eDiscovery công cụ và Commandlets sẽ được nghỉ hưu trong tháng tới:

- [Tại chỗ eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) và [tại chỗ](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) giữ trong Trung tâm quản trị Exchange.

- Các lệnh ghép ngắn Exchange Online PowerShell hỗ trợ tại chỗ eDiscovery và tại chỗ giữ. (Các lệnh ghép ngắn được định dạng chung là *-MailboxSearch lệnh ghép ngắn.) Điều này bao gồm các lệnh ghép ngắn sau đây:

    - [Mới-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Bắt đầu-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Dừng-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Thiết lập MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Lệnh ghép ngắn [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) trong Exchange Online PowerShell.
- Các thao tác sau trong Exchange Web Services API:
    - [Getsearchablehộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonhộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonhộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Văn phòng 365 nâng cao eDiscovery v 1.0](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

**Thời gian cho quỹ hưu**trí:
- Ngày 1 tháng 4 năm 2020: bạn sẽ không thể tạo các tìm kiếm mới và giữ, nhưng bạn vẫn có thể chạy, chỉnh sửa và xóa các tìm kiếm hiện có có nguy cơ của riêng bạn. Microsoft support sẽ không còn hỗ trợ tại chỗ eDiscovery & giữ trong EAC.

- Ngày 1 tháng 7 năm 2020: tại chỗ eDiscovery & giữ chức năng trong EAC sẽ được đặt ở chế độ chỉ đọc. Điều này có nghĩa là bạn chỉ có thể xóa các tìm kiếm hiện có và giữ.

Để biết **thêm thông tin, xem**:

 - [Di chuyển tìm kiếm eDiscovery hợp lệ và giữ cho Trung tâm tuân thủ Microsoft 365](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Nghỉ hưu của công cụ eDiscovery di sản](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Câu hỏi thường gặp về tại chỗ eDiscovery và tại chỗ giữ](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



