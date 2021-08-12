---
title: Tạo nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929327"
---
# <a name="create-a-group"></a>Tạo nhóm

Chủ đề này mô tả cách tạo nhóm.

**Quyền Tạo Nhóm**

Đảm bảo bạn được phép tạo một nhóm mới. Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Panel Truy nhập. Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc cung cấp cho bạn các quyền thích hợp.

**Quản lý quyền tạo Nhóm**

1. Người quản trị toàn cầu có thể quản lý quyền tạo nhóm (vì lý do liên quan bảo mật) hoặc các nhóm Office 365 được tạo trong cổng thông tin Azure hoặc Panel Truy nhập, bằng cách chọn "Người dùng có thể tạo nhóm bảo mật trong cổng thông tin Azure" hoặc tùy chọn "Người dùng có thể tạo nhóm Office 365 trong cổng thông tin Azure" trong Tất cả các nhóm  >  **Chung (Cài đặt).**
2. Bạn cũng có thể hạn chế việc tạo nhóm để chọn nhóm người dùng nếu bạn có giấy Azure Active Directory P1 Premium nhóm.

**Tắt thông báo chào mừng dành cho các thành Office 365 viên nhóm mới**

Thông báo chào mừng được gửi đến những người dùng được thêm vào nhóm Office 365 có thể bị vô hiệu hóa bằng cách đặt **UnifiedGroupWelcomeMessageEnabled** thành False trong Powershell. Tìm hiểu về cài đặt này [tại đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

