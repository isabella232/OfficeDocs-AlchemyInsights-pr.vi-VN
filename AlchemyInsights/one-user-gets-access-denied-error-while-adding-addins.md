---
title: Một người dùng bị từ chối truy cập lỗi khi thêm trình bổ sung trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 1f4672e306a282b3e1d20c75f4e361c02cdddaed
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424283"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="2ebf2-102">Một người dùng bị từ chối truy cập lỗi khi thêm trình bổ sung trong Outlook</span><span class="sxs-lookup"><span data-stu-id="2ebf2-102">One user gets Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="2ebf2-103">Người dùng PowerShell để tìm quyền:</span><span class="sxs-lookup"><span data-stu-id="2ebf2-103">User PowerShell To find permissions:</span></span>

<span data-ttu-id="2ebf2-104">Get-Managementrolegán-RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -delegating $false | Định dạng-bảng-tự động vai trò, RoleAssigneeName, RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="2ebf2-104">Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>