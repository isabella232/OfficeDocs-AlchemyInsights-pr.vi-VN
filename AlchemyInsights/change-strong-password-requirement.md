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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706583"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="9d1fa-102">Thay đổi yêu cầu mật khẩu mạnh</span><span class="sxs-lookup"><span data-stu-id="9d1fa-102">Change strong password requirement</span></span>

<span data-ttu-id="9d1fa-103">Microsoft yêu cầu mật khẩu mạnh theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="9d1fa-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="9d1fa-104">Sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho người dùng cụ thể với lệnh này:</span><span class="sxs-lookup"><span data-stu-id="9d1fa-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="9d1fa-105">*Thiết lập MsolUser-UserPrincipalName <UserPrincipalName> -strongpasswordrequired $false*</span><span class="sxs-lookup"><span data-stu-id="9d1fa-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="9d1fa-106">Thông tin thêm về chính sách mật khẩu</span><span class="sxs-lookup"><span data-stu-id="9d1fa-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="9d1fa-107">Làm thế nào để kết nối với Microsoft 365 với PowerShell</span><span class="sxs-lookup"><span data-stu-id="9d1fa-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="9d1fa-108">Thông tin thêm về lệnh PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="9d1fa-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
