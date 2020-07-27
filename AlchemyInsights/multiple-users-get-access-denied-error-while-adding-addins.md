---
title: Nhiều người dùng có thể truy cập từ chối lỗi khi thêm trình bổ sung trong Outlook
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
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424282"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="8f797-102">Nhiều người dùng có thể truy cập từ chối lỗi khi thêm trình bổ sung trong Outlook</span><span class="sxs-lookup"><span data-stu-id="8f797-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="8f797-103">Bạn có thể chỉ định quản trị viên trong tổ chức của bạn có quyền để cài đặt và quản lý trình bổ sung cho Outlook.</span><span class="sxs-lookup"><span data-stu-id="8f797-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="8f797-104">Bạn cũng có thể chỉ định người dùng nào trong tổ chức của bạn có quyền cài đặt và quản lý trình bổ sung để sử dụng riêng.</span><span class="sxs-lookup"><span data-stu-id="8f797-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="8f797-105">Để biết chi tiết, hãy xem [chỉ định quản trị viên và người dùng có thể cài đặt và quản lý trình bổ sung cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="8f797-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="8f797-106">Để xác minh rằng bạn đã gán thành công các quyền cho người dùng, hãy thay thế <Role Name> bằng tên của vai trò đó để xác minh và chạy lệnh sau trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="8f797-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="8f797-107">Get-Managementrolegán-vai trò " <Role Name> "-geteffectiveusers</span><span class="sxs-lookup"><span data-stu-id="8f797-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="8f797-108">Ví dụ này cho bạn biết cách xác minh người mà bạn đã gán quyền để cài đặt trình bổ sung từ Office Store cho tổ chức.</span><span class="sxs-lookup"><span data-stu-id="8f797-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="8f797-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="8f797-109">PowerShell</span></span>

<span data-ttu-id="8f797-110">-Vai trò "ứng dụng org Marketplace"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="8f797-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="8f797-111">Trong kết quả, Get-Managementrolegán, đánh giá các mục trong cột hiệu quả người dùng.</span><span class="sxs-lookup"><span data-stu-id="8f797-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="8f797-112">Để biết cú pháp chi tiết và thông tin tham số, xem [Get-Managementrolegán](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="8f797-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 