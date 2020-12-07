---
title: 'Vai trò RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584172"
---
# <a name="rbac-rules"></a><span data-ttu-id="32d8e-102">Quy tắc RBAC</span><span class="sxs-lookup"><span data-stu-id="32d8e-102">RBAC rules</span></span>

<span data-ttu-id="32d8e-103">Nếu bạn nhận được lỗi quyền:</span><span class="sxs-lookup"><span data-stu-id="32d8e-103">If you get the permission error:</span></span> 

- <span data-ttu-id="32d8e-104">**Máy khách có ID đối tượng không được phép thực hiện hành động trên phạm vi (mã: ủy quyền không thành công)**: khi bạn tìm cách tạo một tài nguyên, hãy kiểm tra xem bạn đang đăng nhập bằng một người dùng được gán vai trò có quyền viết với tài nguyên ở phạm vi đã chọn.</span><span class="sxs-lookup"><span data-stu-id="32d8e-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="32d8e-105">Ví dụ, để quản lý các máy ảo trong một nhóm tài nguyên, bạn nên có vai trò người [đóng góp máy ảo](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) trên nhóm tài nguyên (hoặc phạm vi mẹ).</span><span class="sxs-lookup"><span data-stu-id="32d8e-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="32d8e-106">Để có danh sách các quyền cho từng vai trò dựng sẵn, hãy xem [vai trò dựng sẵn cho các tài nguyên Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="32d8e-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="32d8e-107">**Bạn không có quyền để tạo yêu cầu hỗ trợ**: khi bạn tìm cách tạo hoặc cập nhật một vé hỗ trợ, hãy kiểm tra xem bạn hiện đang đăng nhập bằng một người dùng được gán vai trò đó là Microsoft. support/supportticket/write Permission, chẳng hạn như bộ [cộng tác yêu cầu hỗ trợ](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="32d8e-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="32d8e-108">**Không có thêm vai trò nào được tạo (mã: RoleAssignmentLimitExceeded)**: khi bạn tìm cách gán vai trò, hãy cố gắng giảm số lượng gán vai trò bằng cách gán vai trò cho các nhóm thay vào đó.</span><span class="sxs-lookup"><span data-stu-id="32d8e-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="32d8e-109">Azure hỗ trợ tối đa **2000** gán vai trò cho mỗi thuê bao.</span><span class="sxs-lookup"><span data-stu-id="32d8e-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="32d8e-110">Để biết thêm chi tiết về các vai trò Azure RBAC, hãy xem các [vai trò AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="32d8e-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
