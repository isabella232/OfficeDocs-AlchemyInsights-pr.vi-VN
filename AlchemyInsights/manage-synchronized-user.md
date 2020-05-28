---
title: Quản lý người dùng đồng bộ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407372"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="58543-102">Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc xóa/xóa người dùng đã đồng bộ hoá</span><span class="sxs-lookup"><span data-stu-id="58543-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="58543-103">Nếu đồng bộ hóa thư mục được kích hoạt cho môi trường của bạn, một số người dùng hoặc đối tượng thuộc tính không thể thay đổi bằng cách sử dụng trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="58543-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="58543-104">Để quản lý đầy đủ người dùng đồng bộ và tất cả các thuộc tính của họ, sử dụng bảng điều khiển quản lý nhóm và người dùng Active Directory của bạn (Adsiedit. msc).</span><span class="sxs-lookup"><span data-stu-id="58543-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="58543-105">Ngoài ra, bạn có thể thay đổi người dùng cá nhân hoặc thuộc tính cho người dùng được đồng bộ hóa bằng cách sử dụng PowerShell như được hiển thị trong các ví dụ phổ biến:</span><span class="sxs-lookup"><span data-stu-id="58543-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
