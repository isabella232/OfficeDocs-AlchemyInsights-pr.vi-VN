---
title: Ẩn các thư mục công cộng
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
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315445"
---
# <a name="hide-public-folders"></a>Ẩn các thư mục công cộng

**Để ẩn toàn bộ cây thư mục công cộng**:

Hãy làm theo các bước trong bài viết [này](https://aka.ms/ControlPF) để ẩn toàn bộ cây thư mục công cộng khỏi chọn lọc hoặc tất cả người dùng.

**Để ẩn một thư mục công cộng cụ thể**:

1. Thêm quyền cho người dùng cần truy nhập vào thư mục công cộng

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Loại bỏ **mặc định** của người dùng khỏi danh sách **quyền** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
