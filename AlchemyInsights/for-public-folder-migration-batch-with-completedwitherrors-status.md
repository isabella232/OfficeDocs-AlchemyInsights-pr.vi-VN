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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068186"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Đối với lô di chuyển thư mục công cộng với trạng thái CompletedWithErrors

Làm theo các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu: 
1. Phê duyệt các mục đã bỏ qua trên lô di chuyển:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Sử dụng lệnh sau đây để phê duyệt các mục đã bỏ qua trên yêu cầu di chuyển được "Đã đồng bộ" nhưng chưa hoàn thành:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Lô di chuyển và yêu cầu sẽ tiếp tục hoạt động lại và hoàn tất trong vài phút.

