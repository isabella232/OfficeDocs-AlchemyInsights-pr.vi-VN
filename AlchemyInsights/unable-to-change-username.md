---
title: Không thể thay đổi tên người dùng
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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798686"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="4a118-102">Không thể thay đổi tên người dùng</span><span class="sxs-lookup"><span data-stu-id="4a118-102">Unable to change UserName</span></span>

<span data-ttu-id="4a118-103">Trong một số trường hợp, UPN (UserPrincipalName) sẽ không được chuyển phát ra trên điện toán đám mây.</span><span class="sxs-lookup"><span data-stu-id="4a118-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="4a118-104">Bạn có thể nhận được các lỗi xác thực trong cổng thông tin Office 365 hoặc không thể thay đổi tên người dùng hoặc địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="4a118-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="4a118-105">Để giải quyết sự cố này, hãy đặt UserPrincipalName theo cách thủ công bằng lệnh PowerShell này.</span><span class="sxs-lookup"><span data-stu-id="4a118-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="4a118-106">**Ví dụ: đổi tên người dùng**</span><span class="sxs-lookup"><span data-stu-id="4a118-106">**Example: Rename a user**</span></span>

<span data-ttu-id="4a118-107">Các PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="4a118-107">PowerShellCopy</span></span>

<span data-ttu-id="4a118-108">PS C: \> Set-MsolUserPrincipalName-UserPrincipalName "DavidC@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="4a118-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="4a118-109">Lệnh này đổi tên DavidC@contoso.com to davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4a118-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="4a118-110">Để biết thêm thông tin, hãy xem [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="4a118-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>