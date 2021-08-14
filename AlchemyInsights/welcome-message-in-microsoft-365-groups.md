---
title: Thông điệp chào mừng trong Microsoft 365 Groups
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
- "5685"
ms.openlocfilehash: 81127b79d4e5a16686ca46d67bfac73c15891938491a702219cd73757c4e106c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997732"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Thông điệp chào mừng trong Microsoft 365 Groups

Những người dùng mới gia Microsoft 365 sẽ nhận được email chào mừng nếu thuộc tính "UnifiedGroupWelcomeMessageEnabled" là True.

Trong trường hợp bạn muốn tắt thông điệp chào mừng, hãy sử dụng lệnh [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) sau đây:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
