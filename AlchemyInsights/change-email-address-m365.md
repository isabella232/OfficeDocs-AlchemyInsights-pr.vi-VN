---
title: Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm
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
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756579"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft nhóm

Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc các nhóm Microsoft bằng cách sử dụng [Trung tâm quản trị microsoft 365](https://admin.microsoft.com/). Chỉ cần chọn Nhóm và chọn @edit địa chỉ email.

Bạn cũng có thể sử dụng lệnh EXO PowerShell sau đây để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365/Nhóm:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Mẫu

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
