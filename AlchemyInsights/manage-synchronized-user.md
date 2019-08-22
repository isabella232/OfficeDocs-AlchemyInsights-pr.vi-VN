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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Không thể đặt địa chỉ email chính hoặc thay đổi các thuộc tính người dùng

Nếu đồng bộ hoá thư mục được kích hoạt cho môi trường của bạn, một số thuộc tính đối tượng hoặc người dùng không thể thay đổi bằng cách sử dụng trung tâm quản trị Microsoft 365.

Để hoàn toàn quản lý người dùng đồng bộ và tất cả các thuộc tính của họ, sử dụng của bạn địa phương hoạt động thư mục người dùng và nhóm quản lý giao diện điều khiển (adsiedit.msc).  

Ngoài ra, bạn có thể thay đổi người dùng cá nhân hoặc các thuộc tính cho người dùng đồng bộ bằng cách sử dụng powershell chẳng hạn như hiển thị trong những ví dụ phổ biến: 
- Thiết lập-MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Thiết lập-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Người dùng kiểm tra" - LastName "Người dùng"-tiêu đề "Quản lý"-vùng "Nhân sự"
- Hủy bỏ-MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com