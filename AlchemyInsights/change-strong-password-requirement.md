---
title: Thay đổi mật khẩu mạnh yêu cầu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701605"
---
# <a name="change-strong-password-requirement"></a>Thay đổi mật khẩu mạnh yêu cầu

Mật khẩu mạnh bắt buộc theo mặc định. 

Bằng cách sử dụng PowerShell bạn có thể vô hiệu hóa các mật khẩu mạnh mẽ cho người dùng cụ thể với lệnh này:<br>
*Thiết lập-MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Thông tin thêm về chính sách mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Làm thế nào để kết nối với O365 bằng PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Thêm thông tin về lệnh PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)