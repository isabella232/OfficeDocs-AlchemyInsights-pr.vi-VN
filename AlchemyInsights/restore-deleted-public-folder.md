---
title: Khôi phục thư mục công cộng đã xóa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158552"
---
# <a name="restore-a-deleted-public-folder"></a>Khôi phục thư mục công cộng đã xóa

**Để khôi phục các mục đã xóa từ thư mục công cộng**:

- Xem [bạn không thể khôi phục các mục đã xóa từ thư mục công cộng không thư trong Outlook 2016](https://aka.ms/pfrec).
 
**Để khôi phục thư mục công cộng đã bị xóa (của bất kỳ loại nào)**: 

- Vui lòng sử dụng lệnh EXO PowerShell sau:

    Cú pháp:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Ví dụ: lệnh sau sẽ khôi phục Subfolder1 và nơi nó dưới \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.
