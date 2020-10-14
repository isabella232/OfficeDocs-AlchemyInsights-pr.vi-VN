---
title: Quản lý người dùng đã đồng bộ
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451422"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="1b61c-102">Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc loại bỏ/xóa người dùng đã đồng bộ hóa</span><span class="sxs-lookup"><span data-stu-id="1b61c-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="1b61c-103">Nếu đồng bộ hóa thư mục được kích hoạt cho môi trường của bạn, một số thuộc tính người dùng hoặc đối tượng không thể thay đổi bằng cách dùng Trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1b61c-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="1b61c-104">Để quản lý đầy đủ người dùng được đồng bộ hóa và tất cả các thuộc tính của họ, hãy sử dụng bảng điều khiển người dùng Active Directory của bạn và nhóm quản lý nhóm (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="1b61c-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="1b61c-105">Ngoài ra, bạn có thể thay đổi người dùng hoặc thuộc tính riêng lẻ cho người dùng được đồng bộ hóa bằng cách sử dụng PowerShell chẳng hạn như minh họa trong những ví dụ chung này:</span><span class="sxs-lookup"><span data-stu-id="1b61c-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
