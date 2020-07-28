---
title: Không thể thay đổi tên người dùng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440293"
---
# <a name="unable-to-change-username"></a>Không thể thay đổi tên người dùng

Trong một số trường hợp, các thay đổi UPN (UserPrincipalName) không chuyển sang đám mây. Bạn có thể nhận được lỗi soát hợp lệ trong cổng Office 365 hoặc không thể thay đổi tên người dùng hoặc địa chỉ email. Để giải quyết vấn đề này, tự đặt UserPrincipalName bằng cách sử dụng lệnh PowerShell này.

**Ví dụ: đổi tên người dùng**

Máy PowerShellCopy

PS C: \> thiết lập MsolUserPrincipalName-UserPrincipalName "DavidC@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"

Lệnh này đổi tên DavidC@contoso.com để davidchew@contoso.com.

Để biết thêm thông tin, xem [thiết lập MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).