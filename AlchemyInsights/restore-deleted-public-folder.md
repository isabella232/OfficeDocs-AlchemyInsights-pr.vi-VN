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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943397"
---
# <a name="restore-a-deleted-public-folder"></a>Khôi phục thư mục công cộng đã xóa

**Để khôi phục các mục đã xóa từ một thư mục công cộng:**

- Xem [mục Bạn không thể phục hồi các mục đã xóa từ thư mục công cộng không phải thư trong Outlook 2016.](https://aka.ms/pfrec)
 
**Để khôi phục thư mục công cộng đã xóa (thuộc bất kỳ loại nào)**: 

- Vui lòng sử dụng lệnh EXO PowerShell sau:

    Cú pháp:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Ví dụ: Lệnh sau đây sẽ khôi phục Thư mục con1 và đặt nó bên dưới \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Hãy xem [Khôi phục thư mục công cộng đã xóa để](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) biết thêm chi tiết.
