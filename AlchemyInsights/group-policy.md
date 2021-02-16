---
title: Chính sách Nhóm
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256911"
---
# <a name="group-policy"></a>Chính sách Nhóm

Thiết đặt cho các đối tượng người dùng và máy tính trong Azure Active Directory Services (Azure AD DS) thường được quản lý bằng các đối tượng chính sách Nhóm (GPOs). Azure AD DS bao gồm tích hợp sẵn trong GPOs cho người dùng và các bộ chứa máy tính của Hh_ngá. Bạn có thể tùy chỉnh các GPOs tích hợp sẵn để cấu hình chính sách nhóm khi cần thiết cho môi trường của bạn. Các thành viên của nhóm người quản trị Azure AD DC có các đặc quyền quản trị chính sách nhóm trong tên miền Azure AD DS và cũng có thể tạo các đơn vị GPOs và tổ chức tùy chỉnh (ơ). Để biết thêm thông tin về chính sách nhóm là gì và cách thức hoạt động, hãy xem [tổng quan về chính sách Nhóm](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

Trong môi trường hỗn hợp, chính sách nhóm được cấu hình trong môi trường AD DS tại cơ sở không được đồng bộ hóa với Azure AD DS. Để xác định thiết đặt cấu hình cho người dùng hoặc máy tính trong Azure AD DS, hãy chỉnh sửa một trong các phần mặc định của GPOs hoặc tạo một GPO tùy chỉnh.

Bài viết này [quản lý chính sách Nhóm](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) hướng dẫn bạn cách cài đặt công cụ quản lý chính sách nhóm, làm thế nào tấn chỉnh sửa GPOs tích hợp sẵn và cách tạo GPOs tùy chỉnh.



