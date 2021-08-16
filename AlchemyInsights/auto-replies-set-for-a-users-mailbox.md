---
title: Đặt trả lời tự động cho hộp thư
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 85b7e969032607216c948532dcdf83ba09022c7cdfaebce8671c6d2e8fef183d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046634"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Đặt trả lời tự động cho hộp thư của người dùng

**Phương pháp 1**

1. Đăng nhập vào cổng thông Microsoft 365 bạn.

2. Đi tới **Người dùng > dùng hiện** hoạt (hoặc Nhóm > **thư** chung nếu bạn đặt tùy chọn này trên hộp thư chung).

3. Chọn người dùng có hộp thư Microsoft Exchange.

4. Ở menu bay ra ở bên phải, đi đến Cài đặt thư **>** Trả lời  tự động (nếu đó là hộp thư chung, chỉ cần bấm vào Trả lời tự động khi bay ra).

**Phương pháp 2**

1. Đăng nhập vào cổng thông tin quản Microsoft 365 quản trị viên của bạn bằng cách sử dụng thông tin đăng nhập của người quản trị.

2. Bung **rộng Trung tâm Quản** trị , rồi bấm **Exchange.**

3. Bấm vào ảnh ở góc trên bên phải, bấm vào **Một Người** dùng Khác , rồi chọn hộp thư người dùng mà bạn muốn thay đổi.

4. Ở bên trái, chọn Tùy **chọn**, **bấm Sắp xếp Email,** rồi bấm Trả lời tự **động.**

**Phương pháp 3**

Chạy lệnh ghép ngắn sau đây Exchange Online PowerShell:

PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Để biết thêm thông tin về lệnh ghép ngắn này, [hãy xem Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
