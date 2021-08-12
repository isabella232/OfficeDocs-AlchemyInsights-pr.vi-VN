---
title: Các sự cố khi sử dụng bảng điều khiển quản trị Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 9310e8685a922207be8d5672d7929e19313cbb57e0fa6d25de149106692e811f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944153"
---
# <a name="problems-using-the-intune-admin-console"></a>Các sự cố khi sử dụng bảng điều khiển quản trị Intune

**"Truy nhập bị từ chối" khi dẫn hướng cổng thông tin quản trị Intune.**

- Nếu bạn là thành viên của vai trò tùy chỉnh Intune, hãy đảm bảo rằng giấy phép Intune hoặc Enterprise Mobility Suite (EMS) được gán cho tài khoản của bạn.
- Nếu bạn đang sử dụng Trình quản lý Cấu hình để quản lý thiết bị, hãy xác nhận rằng bạn không phải là một phần của tuyển tập người dùng Intune dành cho MDM Trình quản lý Cấu hình.
- Hãy xác minh rằng bạn đã được gán quyền kiểm soát quản trị dựa trên vai trò (RBAC) thích hợp trong lưỡi vai trò Intune.
- Xác nhận rằng nhóm đã dùng không phải là danh sách phân phối. Intune trong cổng thông tin Azure chỉ hỗ trợ tài khoản người dùng thuộc Azure Active Directory nhóm bảo mật. Xem lại các nhóm của bạn trong Cổng thông tin Azure > **Nhóm Intune** hoặc trong cổng thông  >  tin Azure > **Azure Active Directory**.

**Người dùng có quá nhiều quyền đối với vai trò Intune được gán**

Hướng dẫn người dùng truy nhập **Vai trò**  >  **Intune Intune của tôi Quyền**  >  **của tôi Xuất**  >  **để** xem lại các quyền đã cấp.

**Tôi đã thêm nhóm phạm vi vào vai trò, nhưng người dùng với vai trò đó vẫn nhìn thấy những người dùng hoặc thiết bị khác.**

Nhóm phạm vi không lọc bỏ người dùng hoặc thiết bị. Nhóm phạm vi:

- Giới hạn người dùng có thể gán chính sách hoặc ứng dụng.
- Chỉ cho phép những người dùng cụ thể chạy tác vụ từ xa trên thiết bị.

Để biết thêm thông tin về nhóm phạm vi, hãy xem Kiểm soát truy nhập dựa trên vai [trò (RBAC) với Microsoft Intune.](https://docs.microsoft.com/intune/role-based-access-control)

**Tôi đã thêm người dùng vào vai trò Intune nhưng họ vẫn có toàn quyền truy nhập vào bảng điều khiển quản trị Intune.**

Dẫn hướng đến Intune  > Người dùng trong cổng thông tin Azure, rồi xác minh rằng người dùng không được gán cho bất kỳ vai trò nào sau đây trong cổng thông tin Azure:

- Người quản trị toàn cầu
- Người quản trị dịch vụ Intune
- SharePoint quản trị viên

Để biết thêm thông tin, [hãy xem mục Kiểm soát truy nhập dựa trên vai trò (RBAC) với Microsoft Intune.](https://docs.microsoft.com/intune/role-based-access-control)

**Sự cố truy nhập**

Để biết thêm thông [tin, xem mục Bạn không thể đăng nhập vào Office 365, Azure hoặc Intune.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)