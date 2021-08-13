---
title: Sự cố cung cấp SCIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: dc2068bbfde7b633e75b3d42f597cee8e4e5f5a72fbf22ebd6c2d0b768945dc9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061670"
---
# <a name="scim-provisioning-issue"></a>Sự cố cung cấp SCIM

Việc cung cấp tự động đề cập đến việc tạo định danh người dùng và vai trò trong các ứng dụng điện toán đám mây mà người dùng cần truy nhập. Ngoài việc tạo danh tính người dùng, việc cung cấp tự động còn bao gồm việc bảo trì và loại bỏ danh tính người dùng khi trạng thái hoặc vai trò thay đổi. Trước khi bắt đầu triển [](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) khai, bạn có thể xem lại Cách việc cung cấp hoạt động để tìm hiểu cách hoạt động của việc cung cấp Azure Active Directory (AD) và nhận các đề xuất về cấu hình.

Với tư cách là nhà phát triển ứng dụng, bạn có thể sử dụng API quản lý Danh tính Chéo Miền (SCIM) để bật chức năng tự động cung cấp người dùng và nhóm giữa ứng dụng của bạn và Azure AD. Bài viết Xây dựng điểm cuối [SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) và đặt cấu hình việc cung cấp người dùng bằng Azure AD mô tả cách xây dựng một điểm cuối SCIM và tích hợp điểm cuối đó với dịch vụ cung cấp Azure AD.



