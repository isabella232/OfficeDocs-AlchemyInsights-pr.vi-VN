---
title: Đối với lô di chuyển thư mục công cộng với trạng thái CompletedWithErrors
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744135"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Đối với lô di chuyển thư mục công cộng với trạng thái CompletedWithErrors

Hãy làm theo các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu: 
1. Phê duyệt các mục đã bỏ qua trên lô di chuyển:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Sử dụng lệnh sau đây để phê duyệt các mục đã bỏ qua trong yêu cầu di chuyển được "được đồng bộ hóa" nhưng chưa hoàn thành:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Lô di chuyển và yêu cầu nên tiếp tục và hoàn thành trong vài phút.

