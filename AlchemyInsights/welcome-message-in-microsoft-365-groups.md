---
title: Thư chào mừng trong Microsoft 365 nhóm
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
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358332"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Thư chào mừng trong Microsoft 365 nhóm

Người dùng mới gia nhập Microsoft 365 Group sẽ nhận được email chào mừng nếu thuộc tính "UnifiedGroupWelcomeMessageEnabled" là đúng.

Trong trường hợp bạn muốn vô hiệu hoá thư chào mừng, sử dụng lệnh [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) sau:

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
