---
title: Một người dùng không nhìn thấy các phần bổ trợ trong Outlook
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
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050680"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Một người dùng không nhìn thấy các phần bổ trợ trong Outlook

Người dùng có thể là một phần của vai trò không có tham số AppsForOfficeEnabled chính xác. Chạy lệnh ghép ngắn này để tìm hiểu xem vai trò chính xác có được liên kết với người dùng hay không:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Ủy quyền $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

Để biết thêm thông tin, xem mục Chỉ định người quản trị và người dùng có thể cài đặt và [quản lý phần bổ trợ cho Outlook.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)
