---
title: Các thư được gửi đến nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên
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
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806169"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Các thư được gửi đến một nhóm Microsoft 365 sẽ không nhận được tất cả các thành viên

Hãy đảm bảo rằng tất cả các thành viên nhóm đã đăng ký nhận email. Xem [theo dõi một nhóm trong Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Để kiểm tra trạng thái thư của những thành viên đã đăng ký với email nhóm, hãy chạy lệnh sau đây trên [eXo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`