---
title: Thông điệp Chào mừng trong nhóm Microsoft 365
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
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725861"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Thông điệp Chào mừng trong nhóm Microsoft 365

Người dùng mới gia nhập nhóm Microsoft 365 sẽ nhận được email chào mừng nếu thuộc tính "UnifiedGroupWelcomeMessageEnabled" là true.

Trong trường hợp bạn muốn vô hiệu hóa thư chào mừng, hãy dùng lệnh [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) sau đây:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
