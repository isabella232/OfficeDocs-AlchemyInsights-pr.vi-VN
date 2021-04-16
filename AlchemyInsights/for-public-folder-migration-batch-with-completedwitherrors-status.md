---
title: Đối với lô di chuyển thư mục công cộng với trạng thái CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812486"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Đối với lô di chuyển thư mục công cộng với trạng thái CompletedWithErrors

Hãy làm theo các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu: 
1. Phê duyệt các mục đã bỏ qua trên lô di chuyển:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Sử dụng lệnh sau đây để phê duyệt các mục đã bỏ qua trong yêu cầu di chuyển được "được đồng bộ hóa" nhưng chưa hoàn thành:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Lô di chuyển và yêu cầu nên tiếp tục và hoàn thành trong vài phút.

