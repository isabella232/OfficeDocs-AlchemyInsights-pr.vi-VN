---
title: Một người dùng không nhìn thấy phần bổ trợ trong Outlook
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
ms.openlocfilehash: 8c99b443a2d83f3ac24362d63cd6363a66a81393
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719687"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Một người dùng không nhìn thấy phần bổ trợ trong Outlook

Người dùng có thể là một phần của một vai trò không có tham số kích hoạt Appsforofficeđúng. Chạy lệnh ghép ngắn này để tìm hiểu xem vai trò chính xác được liên kết với người dùng không:

Get-Managementrolegán-RoleAssignee user@domain.com-Deletưới $false | Định dạng-đóng vai trò tự động, RoleAssigneeName, RoleAssigneeType

Để biết thêm thông tin, hãy xem [mục xác định người quản trị và người dùng có thể cài đặt và quản lý các phần bổ trợ cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
