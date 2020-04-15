---
title: Đặt trả lời tự động cho hộp thư của người dùng
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506654"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Đặt trả lời tự động cho hộp thư của người dùng

**Phương pháp 1**

1. Đăng nhập vào cổng Office 365.

2. Truy cập **người dùng > người dùng đang hoạt động** (hoặc **nhóm > hộp thư dùng chung** nếu bạn đặt điều này vào hộp thư dùng chung).

3. Chọn một người dùng có hộp thư Microsoft Exchange.

4. Trên menu Fly-out ở bên phải, đi tới **cài đặt Mail > trả lời tự động** (nếu đó là hộp thư dùng chung, chỉ cần nhấp vào **trả lời tự động** trên Fly-out).

**Phương pháp 2**

1. Đăng nhập vào cổng quản trị Office 365 bằng cách sử dụng uỷ nhiệm quản trị viên.

2. Mở rộng **Trung tâm quản trị**, và sau đó bấm **Exchange**.

3. Bấm vào hình ảnh ở góc trên bên phải, bấm **người dùng khác**, và sau đó chọn hộp thư người dùng mà bạn muốn thay đổi.

4. Ở bên trái, chọn **tuỳ chọn**, bấm **tổ chức E-mail**, và sau đó nhấp vào **trả lời tự động.**

**Phương pháp 3**

Chạy lệnh sau trong Exchange Online PowerShell:

Máy PowerShellCopy

    Set-MailboxAutoReplyConfiguration

Để biết thêm thông tin về lệnh này, xem [thiết lập MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
