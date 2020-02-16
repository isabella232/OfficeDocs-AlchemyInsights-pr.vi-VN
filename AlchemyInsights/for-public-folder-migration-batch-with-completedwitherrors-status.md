---
title: Thư mục công cộng lô di chuyển với trạng thái Completedwithlỗi
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
- "3532"
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043631"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Thư mục công cộng lô di chuyển với trạng thái Completedwithlỗi

Sử dụng các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu: 
1. Phê duyệt các mục đã bỏ qua trên lô di chuyển:

    Thiết lập MigrationBatch \<batchname>-ApproveSkippedItems 
2. Sử dụng lệnh sau để phê duyệt các mục đã bỏ qua yêu cầu di chuyển "đồng bộ hóa" nhưng không hoàn thành:

    $pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i trong $pf) {if ($i. LargeItemsEncountered-gt 0-hoặc $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}
3. Lô di chuyển và yêu cầu nên tiếp tục và hoàn thành trong vài phút.

