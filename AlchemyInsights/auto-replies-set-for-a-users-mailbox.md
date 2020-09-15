---
title: Đặt trả lời tự động cho một hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715151"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Đặt trả lời tự động cho hộp thư của người dùng

**Phương pháp 1**

1. Đăng nhập vào cổng thông tin Microsoft 365.

2. Đi tới **người dùng > người dùng hiện hoạt** (hoặc **nhóm > hộp thư chung** nếu bạn đặt này trên hộp thư chung).

3. Chọn một người dùng có hộp thư Microsoft Exchange.

4. Trên menu bay ra ở bên phải, hãy đi đến **thiết đặt thư > trả lời tự động** (nếu đó là hộp thư chung, chỉ cần bấm vào **trả lời tự động** trên đường bay).

**Phương pháp 2**

1. Đăng nhập vào cổng thông tin quản trị Microsoft 365 bằng thông tin xác thực người quản trị.

2. Bung rộng **Trung tâm quản trị**, rồi bấm vào **Exchange**.

3. Bấm vào ảnh ở góc trên bên phải, bấm vào **một người dùng khác**, rồi chọn hộp thư người dùng mà bạn muốn thay đổi.

4. Ở bên trái, chọn **tùy chọn**, bấm vào **sắp xếp email**, rồi bấm **trả lời tự động.**

**Phương pháp 3**

Chạy lệnh ghép ngắn sau đây trong Exchange Online PowerShell:

Các PowerShellCopy

```
    Set-MailboxAutoReplyConfiguration
```

Để biết thêm thông tin về lệnh ghép ngắn này, hãy xem mục [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
