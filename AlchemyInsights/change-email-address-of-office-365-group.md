---
title: Thay đổi địa chỉ email của Microsoft 365 nhóm
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
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930751"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Thay đổi địa chỉ email của Microsoft 365 nhóm

Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 nhóm bằng cách sử dụng trung tâm quản trị. Chỉ cần chọn nhóm và chọn @edit chỉ email.

Bạn cũng có thể sử dụng sau lệnh EXO PowerShell để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365 tiên:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Ví dụ:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
