---
title: Thay đổi địa chỉ email của Microsoft 365 hoặc nhóm Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995644"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Thay đổi địa chỉ email của Microsoft 365 hoặc nhóm Microsoft Teams

Bạn có thể thay đổi địa chỉ email của một nhóm Microsoft 365 hoặc Microsoft Teams bằng cách [sử](https://admin.microsoft.com/)dụng Trung tâm quản trị Microsoft 365. Chỉ cần chọn nhóm và chọn @edit chỉ email.

Bạn cũng có thể sử dụng lệnh EXO PowerShell sau đây để thay đổi địa chỉ SMTP chính của một nhóm Microsoft 365/Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Ví dụ:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
