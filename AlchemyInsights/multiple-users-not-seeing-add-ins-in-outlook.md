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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729893"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Nhiều người dùng không nhìn thấy phần bổ trợ trong Outlook

Nếu bạn kiểm tra phần bổ trợ Outlook và không hiển thị, làm bước khắc phục sự cố đầu tiên, hãy sử dụng lệnh ghép ngắn **Get-OrganizationConfig** PowerShell để truy vấn tham số _kích hoạt appsforofficeenabled_ . Nếu truy vấn trả về một giá trị **false**, hãy đặt tham số này thành **True** bằng lệnh ghép ngắn **Set-OrganizationConfig** , do đó, phần bổ trợ sẽ xuất hiện như mong muốn.

Chúng tôi không khuyên bạn nên tham biến cho _phép Appsforofficeđược_ đặt thành **false**. Một giá trị **false** sẽ đè lên tất cả các thiết đặt vai trò quản trị và người dùng và ngăn không cho bất kỳ ứng dụng nào mới được kích hoạt bởi bất kỳ người dùng nào trong tổ chức.

Để biết thêm thông tin, hãy xem [mục xác định người quản trị và người dùng có thể cài đặt và quản lý các phần bổ trợ cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).