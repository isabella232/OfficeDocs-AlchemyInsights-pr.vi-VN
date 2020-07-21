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
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="7c15a-102">Người dùng duy nhất không thấy trình bổ sung trong Outlook</span><span class="sxs-lookup"><span data-stu-id="7c15a-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="7c15a-103">Người dùng có thể là một phần của một vai trò không có tham số AppsForOfficeEnabled chính xác.</span><span class="sxs-lookup"><span data-stu-id="7c15a-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="7c15a-104">Chạy lệnh này để tìm hiểu xem đúng vai trò được liên kết với người dùng:</span><span class="sxs-lookup"><span data-stu-id="7c15a-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="7c15a-105">Get-Managementrolegán-RoleAssignee user@domain.com-Delegating $false | Định dạng-bảng-tự động vai trò, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="7c15a-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="7c15a-106">Để biết thêm thông tin, [hãy xem chỉ định quản trị viên và người dùng có thể cài đặt và quản lý trình bổ sung cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="7c15a-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
