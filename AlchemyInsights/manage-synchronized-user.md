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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542039"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="44f8c-102">Không thể đặt địa chỉ email chính hoặc thay đổi các thuộc tính người dùng</span><span class="sxs-lookup"><span data-stu-id="44f8c-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="44f8c-103">Nếu đồng bộ hoá thư mục được kích hoạt cho môi trường của bạn, một số thuộc tính đối tượng hoặc người dùng không thể thay đổi bằng cách sử dụng trung tâm quản trị Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="44f8c-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="44f8c-104">Để hoàn toàn quản lý người dùng đồng bộ và tất cả các thuộc tính của họ, sử dụng của bạn địa phương hoạt động thư mục người dùng và nhóm quản lý giao diện điều khiển (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="44f8c-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="44f8c-105">Ngoài ra, bạn có thể thay đổi người dùng cá nhân hoặc các thuộc tính cho người dùng đồng bộ bằng cách sử dụng powershell chẳng hạn như hiển thị trong những ví dụ phổ biến:</span><span class="sxs-lookup"><span data-stu-id="44f8c-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="44f8c-106">Thiết lập-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="44f8c-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="44f8c-107">Thiết lập-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Người dùng kiểm tra" - LastName "Người dùng"-tiêu đề "Quản lý"-vùng "Nhân sự"</span><span class="sxs-lookup"><span data-stu-id="44f8c-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="44f8c-108">Hủy bỏ-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="44f8c-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>