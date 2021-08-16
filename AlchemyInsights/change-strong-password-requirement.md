---
title: Thay đổi Yêu cầu mật khẩu Mạnh
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
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070706"
---
# <a name="change-strong-password-requirement"></a>Thay đổi yêu cầu mật khẩu mạnh

Microsoft yêu cầu mật khẩu mạnh theo mặc định.

Bằng cách sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho những người dùng cụ thể với các lệnh sau:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Để vô hiệu hóa mật khẩu mạnh cho tất cả người dùng, hãy sử dụng:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Thông tin thêm về chính sách mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Cách kết nối với Microsoft 365 với PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Thông tin thêm về các lệnh PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
