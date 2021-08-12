---
title: Cách thêm và quản lý người quản trị - các bước được đề xuất
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
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963809"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Cách thêm và quản lý người quản trị - các bước được đề xuất

Dựa trên mô tả sự cố của bạn, chúng tôi đã tìm thấy giải pháp cho bạn. Hầu hết khách hàng đều có thể tự khắc phục sự cố sau khi làm theo hướng dẫn sử dụng của chúng tôi.

**Chỉnh sửa Người quản trị Đăng ký hoặc Người đồng quản trị**

- Người quản trị Tài khoản có thể chỉnh sửa cả hai vai trò này, trong khi Người quản trị Đăng ký chỉ có thể thay đổi Người quản trị đồng quản trị trong [cổng thông tin Azure.](https://ms.portal.azure.com/#home)
- [Thêm hoặc thay đổi người quản trị gói đăng ký Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Cập nhật Người quản trị Đăng ký hoặc Co-Administrator cho Đăng ký Nội bộ (AIRS)**

Người quản trị Dịch vụ hoặc Người quản trị đồng có thể tự phục vụ hành động này bằng cách sử dụng các bước sau đây:

1. Đăng nhập vào cổng thông [tin Azure và](https://ms.portal.azure.com/#home) bấm vào Quản lý Chi phí + **Thanh** toán bằng lưỡi bên trái.
2. Bấm vào mục dòng với gói đăng ký của bạn. Điều này sẽ mở Tổng quan cho đăng ký của bạn.
3. Trên **lưỡi Đăng** ký, bấm vào **Thuộc tính**. 
4. Bấm vào nút **Người quản trị Dịch** vụ.
5. Nhập email của người dùng mà bạn muốn đặt làm Người quản trị Dịch vụ và bấm **OK.**

**Thêm/Thay đổi/Loại bỏ Người đồng quản trị**

1. Đăng nhập vào cổng thông [tin Azure với tư](https://ms.portal.azure.com/#home) cách là Người quản trị Dịch vụ.
2. Mở [Đăng ký và](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) chọn một đăng ký. (Chỉ có thể chỉ định người đồng quản trị ở phạm vi đăng ký.)
3. Dẫn hướng đến kiểm soát **Access (IAM)** Người quản trị cổ điển Thêm Thêm người đồng quản trị để mở ngăn Thêm người đồng quản trị (Nếu tùy chọn Thêm người quản trị đồng bị vô hiệu hóa, tùy chọn này sẽ biểu thị rằng bạn không có  >    >    >   quyền). 
4. Chọn người dùng mà bạn muốn thêm và bấm **Thêm.**

**Tìm hiểu thêm:**
- [Thêm Người đồng quản trị](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Loại bỏ người đồng quản trị](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Thay đổi Người quản trị Dịch vụ](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Xem Người quản trị Tài khoản](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Quản lý quyền truy nhập bằng RBAC và cổng thông tin Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Thêm/xóa người dùng bằng cách sử Azure Active Directory (AD)**

Bạn có thể thêm người dùng mới hoặc xóa người dùng hiện có khỏi tổ chức Azure Active Directory (Azure AD) của mình:

1. Để thêm người dùng mới, hãy đăng nhập vào cổng thông [tin Azure với](https://ms.portal.azure.com/#home) tư cách là Người quản trị người dùng cho tổ chức.
2. Chọn Azure Active Directory , chọn Người **dùng,** rồi bấm vào **Người dùng mới.**
3. Trên trang **Người dùng,** hãy điền thông tin bắt buộc. Bấm **vào Tạo**. Người dùng được tạo và thêm vào đối tượng thuê Azure AD của bạn.

**Tìm hiểu thêm:**

- [Thêm người dùng mới](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Xóa người dùng](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Thêm hoặc cập nhật thông tin hồ sơ của người dùng bằng cách Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Tài liệu được đề xuất**

- [Kiểm soát truy nhập dựa trên vai trò (RBAC) là gì?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Hiểu rõ các vai trò khác nhau trong Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Quyền vai trò của người quản trị Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Hướng dẫn: Cấp quyền truy nhập cho người dùng bằng cách sử dụng RBAC và cổng thông tin Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Khắc phục sự cố về RBAC trong Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Sắp xếp tài nguyên của bạn với các nhóm quản lý Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Cách yêu cầu bản sao hóa đơn Azure qua email](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Cách thêm, cập nhật hoặc loại bỏ thẻ tín dụng hoặc thẻ ghi nợ khỏi Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Quản lý (Kích hoạt lại/Hủy bỏ/Chuyển) đăng ký](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



