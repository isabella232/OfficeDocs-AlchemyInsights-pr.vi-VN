---
title: Ẩn thư mục công cộng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945764"
---
# <a name="hide-public-folders"></a>Ẩn thư mục công cộng

**Để ẩn toàn bộ cây thư mục công cộng:**

Sử dụng các bước trong bài [viết này](https://aka.ms/ControlPF) để ẩn toàn bộ cây thư mục công cộng khỏi chọn lọc hoặc tất cả người dùng.

**Để ẩn một thư mục công cộng cụ thể:**

1. Thêm quyền cho người dùng cần truy nhập thư mục công cộng

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Loại bỏ người dùng **Mặc định** khỏi danh **sách quyền:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
