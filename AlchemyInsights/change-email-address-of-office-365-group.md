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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283266"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Thay đổi địa chỉ email của một nhóm Microsoft 365

Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 bằng cách sử dụng trung tâm quản trị. Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.

Bạn cũng có thể sử dụng sau lệnh EXO PowerShell để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365:

Thiết lập UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Ví dụ:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
