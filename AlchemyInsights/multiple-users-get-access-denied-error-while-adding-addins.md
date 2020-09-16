---
title: Nhiều người dùng bị từ chối truy nhập lỗi trong khi thêm phần bổ trợ trong Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724385"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="beb62-102">Nhiều người dùng bị từ chối truy nhập lỗi trong khi thêm phần bổ trợ trong Outlook</span><span class="sxs-lookup"><span data-stu-id="beb62-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="beb62-103">Bạn có thể chỉ định người quản trị nào trong tổ chức của bạn có quyền cài đặt và quản lý các phần bổ trợ cho Outlook.</span><span class="sxs-lookup"><span data-stu-id="beb62-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="beb62-104">Bạn cũng có thể xác định người dùng nào trong tổ chức của bạn có quyền cài đặt và quản lý các phần bổ trợ cho việc sử dụng riêng của họ.</span><span class="sxs-lookup"><span data-stu-id="beb62-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="beb62-105">Để biết chi tiết, hãy xem [mục xác định người quản trị và người dùng có thể cài đặt và quản lý các phần bổ trợ cho Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="beb62-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="beb62-106">Để xác nhận rằng bạn đã gán quyền thành công cho một người dùng, hãy thay thế <Role Name> bằng tên của vai trò đó để xác nhận và chạy lệnh sau đây trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="beb62-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="beb62-107">Get-Managementrolegán vai trò " <Role Name> "-geteffectiveusers</span><span class="sxs-lookup"><span data-stu-id="beb62-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="beb62-108">Ví dụ này cho bạn biết cách xác minh người mà bạn đã gán quyền cài đặt phần bổ trợ từ Office Store cho tổ chức.</span><span class="sxs-lookup"><span data-stu-id="beb62-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="beb62-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="beb62-109">PowerShell</span></span>

<span data-ttu-id="beb62-110">-Vai trò "tổ chức ứng dụng của thị trường"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="beb62-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="beb62-111">Trong các kết quả, Get-Managementrolegán, xem lại các mục nhập trong cột người dùng hiệu quả.</span><span class="sxs-lookup"><span data-stu-id="beb62-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="beb62-112">Để biết thông tin về cú pháp và tham số chi tiết, hãy xem [Get-Managementrolegán](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="beb62-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 