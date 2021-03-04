---
title: Triển khai GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428047"
---
# <a name="gpo-deployment"></a>Triển khai GPO

Thiết đặt cho các đối tượng người dùng và máy tính trong Azure Active Directory Services (Azure AD DS) thường được quản lý bằng các đối tượng chính sách Nhóm (GPOs). Azure AD DS bao gồm tích hợp sẵn trong GPOs cho người dùng và các bộ chứa máy tính của Hh_ngá. Bạn có thể tùy chỉnh các GPOs tích hợp sẵn để cấu hình chính sách nhóm khi cần thiết cho môi trường của bạn. Các thành viên của nhóm người quản trị Azure AD DC có các đặc quyền quản trị chính sách nhóm trong tên miền Azure AD DS và cũng có thể tạo các đơn vị GPOs và tổ chức tùy chỉnh (ơ). Để biết thêm thông tin về chính sách nhóm là gì và cách thức hoạt động, hãy xem [tổng quan về chính sách Nhóm](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Trong môi trường hỗn hợp, chính sách nhóm được cấu hình trong môi trường AD DS tại cơ sở không được đồng bộ hóa với Azure AD DS. Để xác định thiết đặt cấu hình cho người dùng hoặc máy tính trong Azure AD DS, hãy chỉnh sửa một trong các phần mặc định của GPOs hoặc tạo một GPO tùy chỉnh.

Bài viết này [quản lý chính sách Nhóm](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hướng dẫn bạn cách cài đặt công cụ quản lý chính sách nhóm, làm thế nào tấn chỉnh sửa GPOs tích hợp sẵn và cách tạo GPOs tùy chỉnh.
