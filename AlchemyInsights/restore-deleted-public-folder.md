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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063784"
---
# <a name="restore-a-deleted-public-folder"></a>Khôi phục thư mục công cộng đã xóa

**Để khôi phục các mục đã xóa từ thư mục công cộng**:

- Xem [bạn không thể khôi phục các mục đã xóa từ thư mục công cộng không thư trong Outlook 2016](https://aka.ms/pfrec).
 
**Để khôi phục thư mục công cộng đã bị xóa (của bất kỳ loại nào)**: 

- Vui lòng sử dụng lệnh EXO PowerShell sau:

    Cú pháp:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Tên-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<đường dẫn nơi thư mục sẽ được khôi phục>

    Ví dụ: lệnh sau sẽ khôi phục Subfolder1 và nơi nó dưới \Parent1:

    >$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Tên-EQ "Subfolder1"}; Thiết lập PublicFolder $pf. Identity-đường dẫn \Parent1

Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.
