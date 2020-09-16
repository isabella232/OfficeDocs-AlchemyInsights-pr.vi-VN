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
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777699"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc loại bỏ/xóa người dùng đã đồng bộ hóa

Nếu đồng bộ hóa thư mục được kích hoạt cho môi trường của bạn, một số thuộc tính người dùng hoặc đối tượng không thể thay đổi bằng cách dùng Trung tâm quản trị Microsoft 365.

Để quản lý đầy đủ người dùng được đồng bộ hóa và tất cả các thuộc tính của họ, hãy sử dụng bảng điều khiển người dùng Active Directory của bạn và nhóm quản lý nhóm (Adsiedit. msc).  

Ngoài ra, bạn có thể thay đổi người dùng hoặc thuộc tính riêng lẻ cho người dùng được đồng bộ hóa bằng cách sử dụng PowerShell chẳng hạn như minh họa trong những ví dụ chung này: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
