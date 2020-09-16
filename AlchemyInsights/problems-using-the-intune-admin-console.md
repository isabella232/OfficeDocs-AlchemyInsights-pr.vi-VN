---
title: Các vấn đề khi sử dụng bảng điều khiển quản trị InTune
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
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728309"
---
# <a name="problems-using-the-intune-admin-console"></a>Các vấn đề khi sử dụng bảng điều khiển quản trị InTune

**"Access bị từ chối" khi dẫn hướng đến cổng thông tin quản trị InTune.**

- Nếu bạn là thành viên của một vai trò tùy chỉnh InTune, hãy đảm bảo giấy phép InTune hoặc gói phần mềm di động (EMS) được gán cho tài khoản của bạn.
- Nếu bạn đang sử dụng trình quản lý cấu hình để quản lý thiết bị, hãy xác nhận bạn không phải là một phần của tuyển tập người dùng InTune cho MDM trình quản lý cấu hình.
- Xác nhận rằng bạn đã được gán quyền điều khiển quản trị dựa trên vai trò thích hợp (RBAC) cho phép trong lưỡi InTune vai trò.
- Xác nhận nhóm được sử dụng không phải là danh sách phân phối. InTune trong cổng thông tin Azure chỉ hỗ trợ các tài khoản người dùng thuộc về các nhóm bảo mật Azure Active Directory. Xem lại các nhóm của bạn trong cổng thông tin Azure > **InTune**  >  **nhóm**hoặc trong Azure Portal > **Azure Active Directory**.

**Người dùng có quá nhiều quyền đối với vai trò InTune được gán**

Thông báo cho người dùng để đi đến **InTune**điều  >  **chỉnh vai trò**  >  **của tôi**  >  **xuất** quyền để xem lại quyền được cấp.

**Tôi đã thêm một nhóm phạm vi vào vai trò, nhưng người dùng trong vai trò đó vẫn nhìn thấy những người dùng hoặc thiết bị khác.**

Nhóm phạm vi không lọc ra người dùng hoặc thiết bị. Nhóm phạm vi:

- Giới hạn người dùng có thể gán các chính sách hoặc ứng dụng.
- Chỉ cho phép người dùng cụ thể chạy các tác vụ từ xa trên các thiết bị.

Để biết thêm thông tin về các nhóm phạm vi, hãy xem  [kiểm soát truy nhập dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).

**Tôi đã thêm một người dùng vào vai trò InTune nhưng vẫn có quyền truy nhập đầy đủ vào bảng điều khiển quản trị InTune.**

Dẫn hướng đến InTune > **người dùng** trong cổng thông tin Azure và xác nhận rằng người dùng không được gán cho bất kỳ vai trò nào sau đây trong cổng thông tin Azure:

- Người quản trị toàn cầu
- Người quản trị dịch vụ InTune
- Người quản trị SharePoint

Để biết thêm thông tin, hãy xem [kiểm soát truy nhập dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).

**Vấn đề truy nhập**

Để biết thêm thông tin, hãy xem [bạn không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).