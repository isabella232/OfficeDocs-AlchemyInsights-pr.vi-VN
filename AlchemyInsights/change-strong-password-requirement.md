---
title: Thay đổi yêu cầu mật khẩu mạnh
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818490"
---
# <a name="change-strong-password-requirement"></a>Thay đổi yêu cầu mật khẩu mạnh

Microsoft yêu cầu mật khẩu mạnh theo mặc định.

Sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho người dùng cụ thể với các lệnh sau:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Để vô hiệu hóa mật khẩu mạnh cho tất cả người dùng, hãy dùng:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Thông tin thêm về chính sách mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cách kết nối với Microsoft 365 với PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Thông tin thêm về các lệnh MsolUser của PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
