---
title: Chính sách nhóm
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
ms.openlocfilehash: 5bccaedda08e2c948a15c0b32c6f6eeecfc8bd4c4555b25291f294fe5deb3019
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088814"
---
# <a name="group-policy"></a>Chính sách nhóm

Cài đặt tượng người dùng và máy tính trong Azure Active Directory Domain Services (Azure AD DS) thường được quản lý bằng cách sử dụng Đối tượng Chính sách Nhóm (GPOs). Azure AD DS bao gồm các GPOs tích hợp sẵn cho bộ chứa Người dùng AADDC và Máy tính AADDC. Bạn có thể tùy chỉnh các GPOs tích hợp sẵn này để đặt cấu hình chính sách nhóm khi cần cho môi trường của bạn. Các thành viên của nhóm người quản trị Azure AD DC có đặc quyền quản trị chính sách nhóm trong miền Azure AD DS và cũng có thể tạo các GPOs tùy chỉnh và các đơn vị tổ chức (OU). Để biết thêm thông tin về chính sách nhóm là gì và cách hoạt động của chính sách đó, hãy xem [Tổng quan về Chính sách Nhóm.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Trong môi trường kết hợp, các chính sách nhóm được đặt cấu hình trong môi trường AD DS tại chỗ không được đồng bộ hóa với Azure AD DS. Để xác định cài đặt cấu hình cho người dùng hoặc máy tính trong Azure AD DS, hãy chỉnh sửa một trong các GPOs mặc định hoặc tạo một GPO tùy chỉnh.

Bài [viết](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) này Quản lý Chính sách Nhóm cho bạn biết cách cài đặt các công cụ Quản lý Chính sách Nhóm, cách chỉnh sửa các GPU tích hợp sẵn và cách tạo CÁC GPO tùy chỉnh.



