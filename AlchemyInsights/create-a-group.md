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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816394"
---
# <a name="create-a-group"></a>Tạo nhóm

Chủ đề này mô tả việc tạo nhóm.

**Quyền tạo nhóm**

Đảm bảo bạn được ủy quyền để tạo nhóm mới. Người quản trị toàn cầu có thể tắt tính năng tạo nhóm trong cổng thông tin Azure hoặc Pa-nen truy nhập. Bạn có thể cần người quản trị để tạo nhóm mới cho bạn hoặc để cung cấp cho bạn quyền thích hợp.

**Quản lý quyền tạo nhóm**

1. Người quản trị toàn cầu có thể quản lý quyền tạo nhóm (cho các lý do liên quan đến bảo mật) hoặc các nhóm Office 365 được tạo trong Azure Portal hoặc Access Panel, bằng cách chọn "người dùng có thể tạo nhóm bảo mật trong Azure Portals" hoặc "người dùng có thể tạo nhóm Office 365 trong Azure Portals" tùy chọn trong **tất cả các nhóm**  >  **chung (thiết đặt)**
2. Bạn cũng có thể hạn chế tạo nhóm để chọn một nhóm người dùng nếu bạn có giấy phép Azure Active Directory P1 Premium.

**Tắt thông báo chào mừng cho các thành viên nhóm mới của Office 365**

Thông báo chào mừng được gửi đến những người dùng được thêm vào các nhóm Office 365 có thể bị vô hiệu hóa bằng cách đặt **Unifiedgroupwelcomemessageenabled** thành false trong PowerShell. Tìm hiểu về thiết đặt này [ở đây](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

