---
title: Các thư được gửi đến nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479475"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Các thư được gửi đến một nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên

Hãy đảm bảo rằng tất cả các thành viên nhóm đã đăng ký nhận email. Xem [theo dõi một nhóm trong Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Để kiểm tra trạng thái thư của những thành viên đã đăng ký với email nhóm, hãy chạy lệnh sau đây trên [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Sử dụng lệnh EXO PowerShell sau đây để cấu hình tất cả các thành viên nhóm để nhận email được gửi đến nhóm Microsoft 365 trong hộp thư đến của họ:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Ví dụ:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`