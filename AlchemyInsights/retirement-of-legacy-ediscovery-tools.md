---
title: Hưu trí của công cụ eDiscovery kế thừa
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
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798571"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Hưu trí của công cụ eDiscovery kế thừa

Là kết quả của chức năng khám phá điện tử mới và được cải tiến trong Trung tâm tuân thủ Microsoft 365, các công cụ và lệnh ghép ngắn sau đây được thiết kế lại sau đó sẽ được ngừng hoạt động trong những tháng sắp tới:

- [Khám phá điện tử tại chỗ](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) và [tại chỗ giữ](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) trong Trung tâm quản trị Exchange.

- Các lệnh ghép ngắn Exchange Online PowerShell hỗ trợ In-Place khám phá điện tử và In-Place giữ. (Các lệnh ghép ngắn này được xác định chung là lệnh ghép ngắn *-MailboxSearch.) Điều này bao gồm các lệnh ghép ngắn sau đây:

    - [Mới-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Khởi động-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Ngăn chặn-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Thiết đặt-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Lệnh ghép ngắn [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) trong Exchange Online PowerShell.
- Các thao tác sau trong API Exchange Web Services:
    - [Tìm kiếm hộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdonhộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdonhộp thư](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Nâng cao eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Đường thời gian cho quỹ hưu trí**:
- **Ngày 1 tháng 7, 2020** Bạn không còn có thể tạo các tìm kiếm mới và giữ, nhưng bạn có thể chạy, chỉnh sửa và xóa bỏ các tìm kiếm hiện có theo rủi ro của riêng bạn. Hỗ trợ của Microsoft không còn hỗ trợ In-Place khám phá điện tử & giữ trong EAC.
    
- **1 tháng mười, 2020** In-Place khám phá điện tử & giữ chức năng trong EAC sẽ được đặt ở chế độ chỉ đọc, vì vậy bạn chỉ có thể loại bỏ các tìm kiếm hiện có và giữ.

**Để biết thêm thông tin, hãy xem**:

 - [Di chuyển các tìm kiếm khám phá điện tử và giữ lại Trung tâm tuân thủ Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Hưu trí của công cụ eDiscovery kế thừa](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Những câu hỏi thường gặp về In-Place khám phá điện tử và In-Place giữ](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



