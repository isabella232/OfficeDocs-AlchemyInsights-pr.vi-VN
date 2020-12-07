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
# <a name="rbac-rules"></a>Quy tắc RBAC

Nếu bạn nhận được lỗi quyền: 

- **Máy khách có ID đối tượng không được phép thực hiện hành động trên phạm vi (mã: ủy quyền không thành công)**: khi bạn tìm cách tạo một tài nguyên, hãy kiểm tra xem bạn đang đăng nhập bằng một người dùng được gán vai trò có quyền viết với tài nguyên ở phạm vi đã chọn. Ví dụ, để quản lý các máy ảo trong một nhóm tài nguyên, bạn nên có vai trò người [đóng góp máy ảo](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) trên nhóm tài nguyên (hoặc phạm vi mẹ). Để có danh sách các quyền cho từng vai trò dựng sẵn, hãy xem [vai trò dựng sẵn cho các tài nguyên Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Bạn không có quyền để tạo yêu cầu hỗ trợ**: khi bạn tìm cách tạo hoặc cập nhật một vé hỗ trợ, hãy kiểm tra xem bạn hiện đang đăng nhập bằng một người dùng được gán vai trò đó là Microsoft. support/supportticket/write Permission, chẳng hạn như bộ [cộng tác yêu cầu hỗ trợ](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Không có thêm vai trò nào được tạo (mã: RoleAssignmentLimitExceeded)**: khi bạn tìm cách gán vai trò, hãy cố gắng giảm số lượng gán vai trò bằng cách gán vai trò cho các nhóm thay vào đó. Azure hỗ trợ tối đa **2000** gán vai trò cho mỗi thuê bao.

Để biết thêm chi tiết về các vai trò Azure RBAC, hãy xem các [vai trò AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
