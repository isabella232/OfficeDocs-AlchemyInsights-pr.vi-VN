---
title: Người dùng duy nhất không thấy trình bổ sung trong Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198225"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Người dùng duy nhất không thấy trình bổ sung trong Outlook

Người dùng có thể là một phần của một vai trò không có tham số AppsForOfficeEnabled chính xác. Chạy lệnh này để tìm hiểu xem đúng vai trò được liên kết với người dùng:

Get-Managementrolegán-RoleAssignee user@domain.com-Delegating $false | Định dạng-bảng-tự động vai trò, RoleAssigneeName, RoleAssigneeType

Để biết thêm thông tin, [hãy xem chỉ định quản trị viên và người dùng có thể cài đặt và quản lý trình bổ sung cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
