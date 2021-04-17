---
title: Quản lý người dùng đã đồng bộ
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
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823989"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="d9a09-102">Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc loại bỏ/xóa người dùng đã đồng bộ hóa</span><span class="sxs-lookup"><span data-stu-id="d9a09-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="d9a09-103">Nếu đồng bộ hóa thư mục được kích hoạt cho môi trường của bạn, một số thuộc tính người dùng hoặc đối tượng không thể thay đổi bằng cách dùng Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d9a09-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="d9a09-104">Để quản lý đầy đủ người dùng được đồng bộ hóa và tất cả các thuộc tính của họ, hãy sử dụng bảng điều khiển người dùng Active Directory của bạn và nhóm quản lý nhóm (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="d9a09-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="d9a09-105">Ngoài ra, bạn có thể thay đổi người dùng hoặc thuộc tính riêng lẻ cho người dùng được đồng bộ hóa bằng cách sử dụng PowerShell chẳng hạn như minh họa trong những ví dụ chung này:</span><span class="sxs-lookup"><span data-stu-id="d9a09-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
