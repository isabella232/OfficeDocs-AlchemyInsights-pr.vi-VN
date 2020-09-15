---
title: Thay đổi yêu cầu mật khẩu mạnh
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681894"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="97bc1-102">Thay đổi yêu cầu mật khẩu mạnh</span><span class="sxs-lookup"><span data-stu-id="97bc1-102">Change strong password requirement</span></span>

<span data-ttu-id="97bc1-103">Microsoft yêu cầu mật khẩu mạnh theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="97bc1-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="97bc1-104">Sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho người dùng cụ thể với lệnh này:</span><span class="sxs-lookup"><span data-stu-id="97bc1-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="97bc1-105">*Set-MsolUser-UserPrincipalName <UserPrincipalName> – strongpasswordrequi$false*</span><span class="sxs-lookup"><span data-stu-id="97bc1-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="97bc1-106">Thông tin thêm về chính sách mật khẩu</span><span class="sxs-lookup"><span data-stu-id="97bc1-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="97bc1-107">Cách kết nối với Microsoft 365 với PowerShell</span><span class="sxs-lookup"><span data-stu-id="97bc1-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="97bc1-108">Thông tin thêm về các lệnh MsolUser của PowerShell</span><span class="sxs-lookup"><span data-stu-id="97bc1-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
