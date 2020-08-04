---
title: Sự cố bằng cách sử dụng bảng điều khiển dành cho quản trị viên InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555883"
---
# <a name="problems-using-the-intune-admin-console"></a>Sự cố bằng cách sử dụng bảng điều khiển dành cho quản trị viên InTune

**"Truy cập bị từ chối" khi điều hướng cổng quản trị InTune.**

- Nếu bạn là thành viên của vai trò tùy chỉnh InTune, hãy đảm bảo giấy phép InTune hoặc Enterprise Mobility Suite (EMS) được gán cho tài khoản của bạn.
- Nếu bạn đang sử dụng trình quản lý cấu hình để quản lý thiết bị, xác minh bạn không phải là một phần của bộ sưu tập người dùng InTune Configuration Manager MDM.
- Xác minh rằng bạn đã được gán quyền kiểm soát quản trị dựa trên vai trò thích hợp (RBAC) trong vai trò InTune.
- Xác minh nhóm được sử dụng không phải là danh sách phân phối. InTune trong cổng thông tin Azure chỉ hỗ trợ tài khoản người dùng thuộc nhóm bảo mật Azure Active Directory. Đánh giá nhóm của bạn trong cổng Azure > **InTune**  >  **nhóm**hoặc Azure cổng > **Azure Active Directory**.

**Người dùng có quá nhiều quyền cho vai trò InTune được chỉ định**

Tư vấn cho người dùng để đi đến **InTune**  >  **InTune vai trò**  >  **của tôi cho phép**  >  **xuất** để xem xét cấp quyền.

**Tôi đã thêm một nhóm phạm vi vào một vai trò, nhưng người dùng trong vai trò đó vẫn nhìn thấy người dùng hoặc thiết bị khác.**

Phạm vi nhóm không lọc ra người dùng hoặc thiết bị. Phạm vi Nhóm:

- Giới hạn người dùng có thể gán chính sách hoặc ứng dụng.
- Chỉ cho phép người dùng cụ thể chạy tác vụ từ xa trên thiết bị.

Để biết thêm thông tin về phạm vi nhóm, xem [kiểm soát truy cập Dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).

**Tôi đã thêm người dùng vào vai trò InTune nhưng họ vẫn có quyền truy cập đầy đủ vào bảng điều khiển dành cho quản trị viên InTune.**

Điều hướng đến InTune > **người dùng** trong cổng thông tin Azure và xác minh rằng người dùng không được gán cho bất kỳ vai trò sau đây trong cổng Azure:

- Quản trị viên toàn cầu
- Quản trị viên dịch vụ InTune
- Quản trị viên SharePoint

Để biết thêm thông tin, xem [kiểm soát truy cập Dựa trên vai trò (RBAC) với Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).

**Vấn đề truy cập**

Để biết thêm thông tin, [hãy xem bạn không thể đăng nhập vào Office 365, Azure hoặc InTune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).