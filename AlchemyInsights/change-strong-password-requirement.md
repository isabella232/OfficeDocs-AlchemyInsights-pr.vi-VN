---
title: Thay đổi mật khẩu mạnh yêu cầu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518781"
---
# <a name="change-strong-password-requirement"></a>Thay đổi mật khẩu mạnh yêu cầu

Microsoft yêu cầu mật khẩu mạnh bằng cách mặc định. 

Bằng cách sử dụng PowerShell, bạn có thể vô hiệu hóa các mật khẩu mạnh mẽ cho người dùng cụ thể với lệnh này:<br>
*Thiết lập-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Thông tin thêm về chính sách mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Làm thế nào để kết nối với Office 365 bằng PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Thêm thông tin về lệnh PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)