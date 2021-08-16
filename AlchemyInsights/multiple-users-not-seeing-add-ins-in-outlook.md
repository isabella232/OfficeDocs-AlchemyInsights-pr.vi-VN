---
title: Nhiều người dùng không nhìn thấy phần bổ trợ trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011826"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Nhiều người dùng không nhìn thấy phần bổ trợ trong Outlook

Nếu bạn kiểm tra Outlook bổ trợ và không hiển thị, như một bước khắc phục sự cố đầu tiên, hãy dùng lệnh ghép ngắn **Get-OrganizationConfig** PowerShell để truy vấn tham số _AppsForOfficeEnabled._ Nếu truy vấn trả về giá trị **False**, hãy đặt tham số này thành **True** bằng cách sử dụng lệnh ghép ngắn **Set-OrganizationConfig** để các phần bổ trợ xuất hiện như dự kiến.

Chúng tôi khuyên tham số _AppsForOfficeEnabled_ được đặt thành **False.** Giá trị **False** sẽ ghi đè lên tất cả các thiết đặt vai trò Người dùng và Quản trị ở trên, đồng thời ngăn người dùng bất kỳ trong tổ chức kích hoạt mọi ứng dụng mới.

Để biết thêm thông tin, hãy xem Chỉ định người quản trị và người dùng có thể cài đặt và [quản lý các phần bổ trợ dành cho Outlook.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)