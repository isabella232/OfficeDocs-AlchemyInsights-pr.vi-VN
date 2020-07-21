---
title: Nhiều người dùng không thấy trình bổ sung trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198247"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Nhiều người dùng không thấy trình bổ sung trong Outlook

Nếu bạn kiểm tra Outlook Add-in và không hiển thị, như là một bước khắc phục sự cố đầu tiên, sử dụng lệnh ghép ngắn PowerShell **Get-OrganizationConfig** để yêu cầu tham số _Appsforofficeenabled_ . Nếu truy vấn trả lại giá trị **false**, đặt tham số này thành **True** bằng cách sử dụng lệnh ghép ngắn **Set-OrganizationConfig** , vì vậy trình bổ sung xuất hiện như mong đợi.

Chúng tôi khuyến nghị tham số _Appsforofficeenabled_ được đặt thành **false**. Giá trị **sai** ghi đè tất cả các cài đặt vai trò quản trị và người dùng ở trên và ngăn mọi ứng dụng mới được kích hoạt bởi bất kỳ người dùng nào trong tổ chức.

Để biết thêm thông tin, hãy xem [chỉ định quản trị viên và người dùng có thể cài đặt và quản lý trình bổ sung cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).