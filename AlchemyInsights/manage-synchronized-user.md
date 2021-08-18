---
title: Quản lý Người dùng Đã đồng bộ
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
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114806"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Không thể đặt địa chỉ email chính, thay đổi thuộc tính người dùng hoặc loại bỏ/xóa người dùng đã đồng bộ

Nếu đồng bộ hóa thư mục được bật cho môi trường của bạn, một số thuộc tính của người dùng hoặc đối tượng không thể thay đổi bằng cách sử dụng Trung tâm quản trị Microsoft 365.

Để quản lý đầy đủ người dùng được đồng bộ hóa và tất cả các thuộc tính của họ, hãy sử dụng bảng điều khiển quản lý nhóm và người dùng active directory cục bộ của bạn (adsiedit.msc).  

Ngoài ra, bạn có thể thay đổi người dùng cá nhân hoặc thuộc tính cho người dùng được đồng bộ hóa bằng cách sử dụng powershell chẳng hạn như được hiển thị trong các ví dụ phổ biến sau đây:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
