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
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="0a521-102">Thông điệp Chào mừng trong nhóm Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0a521-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="0a521-103">Người dùng mới gia nhập nhóm Microsoft 365 sẽ nhận được email chào mừng nếu thuộc tính "UnifiedGroupWelcomeMessageEnabled" là true.</span><span class="sxs-lookup"><span data-stu-id="0a521-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="0a521-104">Trong trường hợp bạn muốn vô hiệu hóa thư chào mừng, hãy dùng lệnh [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) sau đây:</span><span class="sxs-lookup"><span data-stu-id="0a521-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
