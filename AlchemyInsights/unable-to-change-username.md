---
title: Không thể thay đổi Tên Người dùng
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
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020250"
---
# <a name="unable-to-change-username"></a>Không thể thay đổi Tên Người dùng

Trong một số trường hợp, các thay đổi UPN (UserPrincipalName) sẽ không phát tán lên đám mây. Bạn có thể gặp lỗi xác thực trong cổng thông Office 365 hoặc không thể thay đổi tên người dùng hoặc địa chỉ email. Để giải quyết vấn đề này, hãy đặt UserPrincipalName theo cách thủ công bằng cách sử dụng lệnh PowerShell này.

**Ví dụ: Đổi tên người dùng**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Lệnh này sẽ đổi tên davidc@contoso.com tên thành davidchew@contoso.com.

Để biết thêm thông tin, [hãy xem Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).