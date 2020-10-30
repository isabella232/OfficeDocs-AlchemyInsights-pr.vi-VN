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
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804445"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="fe055-102">Thay đổi yêu cầu mật khẩu mạnh</span><span class="sxs-lookup"><span data-stu-id="fe055-102">Change strong password requirement</span></span>

<span data-ttu-id="fe055-103">Microsoft yêu cầu mật khẩu mạnh theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="fe055-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="fe055-104">Sử dụng PowerShell, bạn có thể vô hiệu hóa mật khẩu mạnh cho người dùng cụ thể với các lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="fe055-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="fe055-105">Để vô hiệu hóa mật khẩu mạnh cho tất cả người dùng, hãy dùng:</span><span class="sxs-lookup"><span data-stu-id="fe055-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="fe055-106">Thông tin thêm về chính sách mật khẩu</span><span class="sxs-lookup"><span data-stu-id="fe055-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="fe055-107">Cách kết nối với Microsoft 365 với PowerShell</span><span class="sxs-lookup"><span data-stu-id="fe055-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="fe055-108">Thông tin thêm về các lệnh MsolUser của PowerShell</span><span class="sxs-lookup"><span data-stu-id="fe055-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
