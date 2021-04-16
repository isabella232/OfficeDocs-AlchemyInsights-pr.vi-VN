---
title: Khôi phục thư mục công cộng đã xóa
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
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809461"
---
# <a name="restore-a-deleted-public-folder"></a>Khôi phục thư mục công cộng đã xóa

**Để khôi phục các mục đã xóa khỏi thư mục công cộng**:

- Xem [bạn không thể khôi phục các mục đã xóa khỏi thư mục công cộng không phải thư trong Outlook 2016](https://aka.ms/pfrec).
 
**Để khôi phục thư mục công cộng đã xóa (trong bất kỳ loại nào)**: 

- Vui lòng dùng lệnh EXO PowerShell sau đây:

    Syntax

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Ví dụ: lệnh sau đây sẽ khôi phục Subfolder1 và đặt nó dưới \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.
