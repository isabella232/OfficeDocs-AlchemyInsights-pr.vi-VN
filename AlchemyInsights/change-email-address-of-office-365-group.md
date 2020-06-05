---
title: Thay đổi địa chỉ email của một nhóm Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580679"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Thay đổi địa chỉ email của một nhóm Microsoft 365

Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 bằng cách sử dụng trung tâm quản trị. Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.

Bạn cũng có thể sử dụng sau lệnh EXO PowerShell để thay đổi địa chỉ SMTP chính của nhóm Microsoft 365:

Thiết lập UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Ví dụ:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
