---
title: Yêu cầu thay đổi mật khẩu mạnh
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
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286300"
---
# <a name="change-strong-password-requirement"></a>Thay đổi yêu cầu mật khẩu mạnh

Microsoft yêu cầu mật khẩu mạnh theo mặc định. 

Sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho người dùng cụ thể với lệnh này:<br>
*Thiết lập MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordrequired $false*

- [Thông tin thêm về chính sách mật khẩu](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Làm thế nào để kết nối với Office 365 với PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Thông tin thêm về lệnh PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Đặt mật khẩu của người dùng cá nhân để không bao giờ hết hạn](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
