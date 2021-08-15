---
title: Tất cả các thành viên Microsoft 365 sẽ không nhận được các thư được gửi cho nhóm
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 73c0fd3eb2f022b1c5917849bae676b748025fb69a3a15ba1389b42a6854db9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976527"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Tất cả các thành viên Microsoft 365 thể nhận được thư được gửi cho một nhóm

Đảm bảo rằng tất cả thành viên nhóm đã đăng ký nhận email. Xem [Theo dõi một nhóm trong Outlook.](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)  

Để kiểm tra trạng thái thư của các thành viên đã đăng ký email nhóm, hãy chạy lệnh sau đây trên [EXO PowerShell:](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Sử dụng lệnh EXO PowerShell sau đây để cấu hình cho tất cả các thành viên nhóm nhận email được gửi đến Microsoft 365 nhóm trong hộp thư đến của họ:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Ví dụ:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`