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
# <a name="unable-to-change-username"></a><span data-ttu-id="9c315-102">Không thể thay đổi tên người dùng</span><span class="sxs-lookup"><span data-stu-id="9c315-102">Unable to change UserName</span></span>

<span data-ttu-id="9c315-103">Trong một số trường hợp, các thay đổi UPN (UserPrincipalName) không chuyển sang đám mây.</span><span class="sxs-lookup"><span data-stu-id="9c315-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="9c315-104">Bạn có thể nhận được lỗi soát hợp lệ trong cổng Office 365 hoặc không thể thay đổi tên người dùng hoặc địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="9c315-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="9c315-105">Để giải quyết vấn đề này, tự đặt UserPrincipalName bằng cách sử dụng lệnh PowerShell này.</span><span class="sxs-lookup"><span data-stu-id="9c315-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="9c315-106">**Ví dụ: đổi tên người dùng**</span><span class="sxs-lookup"><span data-stu-id="9c315-106">**Example: Rename a user**</span></span>

<span data-ttu-id="9c315-107">Máy PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="9c315-107">PowerShellCopy</span></span>

<span data-ttu-id="9c315-108">PS C: \> thiết lập MsolUserPrincipalName-UserPrincipalName "DavidC@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="9c315-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="9c315-109">Lệnh này đổi tên DavidC@contoso.com để davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="9c315-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="9c315-110">Để biết thêm thông tin, xem [thiết lập MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="9c315-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>