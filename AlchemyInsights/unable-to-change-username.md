---
title: Không thể thay đổi tên người dùng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798686"
---
# <a name="unable-to-change-username"></a>Không thể thay đổi tên người dùng

Trong một số trường hợp, UPN (UserPrincipalName) sẽ không được chuyển phát ra trên điện toán đám mây. Bạn có thể nhận được các lỗi xác thực trong cổng thông tin Office 365 hoặc không thể thay đổi tên người dùng hoặc địa chỉ email. Để giải quyết sự cố này, hãy đặt UserPrincipalName theo cách thủ công bằng lệnh PowerShell này.

**Ví dụ: đổi tên người dùng**

Các PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-UserPrincipalName "DavidC@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Lệnh này đổi tên DavidC@contoso.com to davidchew@contoso.com.

Để biết thêm thông tin, hãy xem [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).