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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923153"
---
# <a name="rbac-rules"></a>Quy tắc RBAC

Nếu bạn gặp lỗi về quyền: 

- Máy khách có id đối tượng không được ủy quyền để thực hiện hành động vượt quá phạm vi **(mã: AuthorizationFailed)**: khi bạn tìm cách tạo tài nguyên, hãy kiểm tra xem bạn hiện đang đăng nhập với người dùng được gán vai trò có quyền ghi đối với tài nguyên ở phạm vi đã chọn hay không. Ví dụ, để quản lý máy ảo trong [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) nhóm tài nguyên, bạn nên có vai trò Người đóng góp Máy Ảo trên nhóm tài nguyên (hoặc phạm vi mẹ). Để biết danh sách các quyền cho từng vai trò tích hợp sẵn, hãy xem [mục Các vai trò tích hợp sẵn cho tài nguyên Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Bạn không có quyền tạo yêu cầu hỗ trợ **:** khi tìm cách tạo hoặc cập nhật phiếu hỗ trợ, hãy kiểm tra xem bạn hiện đang đăng nhập với người dùng được gán vai trò có quyền Microsoft.Support/supportTickets/write, chẳng hạn như Người đóng góp Yêu cầu Hỗ trợ [.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Không thể tạo thêm việc gán vai trò **(mã: RoleAssignmentLimitExceeded)**: khi bạn cố gắng gán vai trò, hãy cố gắng giảm số lượng bài tập vai trò bằng cách gán vai trò cho nhóm thay vào đó. Azure hỗ trợ tối đa **2000 vai trò** gán cho mỗi đăng ký.

Để biết thêm chi tiết về vai trò Azure RBAC, hãy [xem mục Vai trò Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
