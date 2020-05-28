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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc xóa/xóa người dùng đã đồng bộ hoá

Nếu đồng bộ hóa thư mục được kích hoạt cho môi trường của bạn, một số người dùng hoặc đối tượng thuộc tính không thể thay đổi bằng cách sử dụng trung tâm quản trị Microsoft 365.

Để quản lý đầy đủ người dùng đồng bộ và tất cả các thuộc tính của họ, sử dụng bảng điều khiển quản lý nhóm và người dùng Active Directory của bạn (Adsiedit. msc).  

Ngoài ra, bạn có thể thay đổi người dùng cá nhân hoặc thuộc tính cho người dùng được đồng bộ hóa bằng cách sử dụng PowerShell như được hiển thị trong các ví dụ phổ biến: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
