---
title: Cách thêm và quản lý các bước được đề xuất
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678866"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Cách thêm và quản lý các bước được đề xuất

**Chỉnh sửa người quản trị đăng ký hoặc người quản trị**

- Người quản trị tài khoản có thể chỉnh sửa cả hai vai trò trong khi người quản trị đăng ký chỉ có thể thay đổi đồng quản trị trong [cổng thông tin Azure](https://ms.portal.azure.com/#home).
- [Thêm hoặc thay đổi người quản trị thuê bao Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Cập Nhật người quản trị đăng ký hoặc Co-Administrator cho đăng ký nội bộ (phát sóng)**

Người quản trị dịch vụ hoặc đồng người quản trị có thể tự phục vụ hành động này bằng cách sử dụng các bước sau đây:

1. Đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) và bấm **quản lý chi phí + thanh toán** trong lưỡi mũi trái.
2. Bấm vào mục dòng với đăng ký của bạn. Điều này sẽ mở tổng quan về đăng ký của bạn.
3. Trên lưỡi **đăng ký** , bấm **thuộc tính**. 
4. Bấm vào nút **quản trị dịch vụ** .
5. Nhập email của người dùng mà bạn muốn đặt làm người quản trị dịch vụ và bấm **OK**.

**Thêm/thay đổi/loại bỏ đồng người quản trị**

1. Đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) với tư cách là người quản trị dịch vụ.
2. Mở [đăng ký](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) và chọn một thuê bao. (Đồng quản trị chỉ có thể gán tại phạm vi thuê bao.)
3. Dẫn hướng đến **điều khiển Access (iam)**  >  người **quản trị cổ điển**  >  **Thêm**  >  **Thêm người quản trị đồng** để mở ngăn **Thêm đồng quản trị** (Nếu tùy chọn thêm đồng người quản trị bị vô hiệu hóa, nó sẽ cho biết rằng bạn không có quyền).
4. Chọn người dùng mà bạn muốn thêm, rồi bấm **Thêm**.

**Tìm hiểu thêm:**
- [Thêm người đồng quản trị](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Loại bỏ người đồng quản trị](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Thay đổi người quản trị dịch vụ](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Xem người quản trị tài khoản](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Quản lý quyền truy nhập bằng cổng thông tin RBAC và Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Thêm/xóa người dùng bằng cách sử dụng Azure Active Directory (quảng cáo)**

Bạn có thể thêm người dùng mới hoặc xóa người dùng hiện có khỏi tổ chức Azure Active Directory (Azure AD):

1. Để thêm người dùng mới, hãy đăng nhập vào [cổng thông tin Azure](https://ms.portal.azure.com/#home) với tư cách là người quản trị người dùng cho tổ chức.
2. Chọn **Azure Active Directory**, chọn **người dùng** rồi bấm **người dùng mới**.
3. Trên trang **người dùng** , điền thông tin bắt buộc. Bấm **tạo**. Người dùng được tạo và thêm vào đối tượng thuê Azure AD của bạn.

**Tìm hiểu thêm**:

- [Thêm người dùng mới](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Xóa người dùng](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Thêm hoặc cập nhật thông tin hồ sơ của người dùng bằng cách sử dụng Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Tài liệu được đề xuất**

- [Điều khiển truy nhập dựa trên vai trò là gì (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Tìm hiểu các vai trò khác nhau trong Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Quyền quản trị vai trò trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Hướng dẫn: cấp quyền truy nhập cho người dùng bằng RBAC và cổng thông tin Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Khắc phục sự cố RBAC trong Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Sắp xếp các tài nguyên của bạn với các nhóm quản lý Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Làm thế nào để yêu cầu bản sao hóa đơn Azure qua email](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Cách thêm, Cập Nhật hoặc loại bỏ thẻ tín dụng hoặc thẻ ghi nợ khỏi Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Quản lý (kích hoạt lại/hủy bỏ/chuyển) đăng ký](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



