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
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158650"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="e5fbc-102">Thư mục công cộng lô di chuyển với trạng thái Completedwithlỗi</span><span class="sxs-lookup"><span data-stu-id="e5fbc-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="e5fbc-103">Sử dụng các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu:</span><span class="sxs-lookup"><span data-stu-id="e5fbc-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="e5fbc-104">Phê duyệt các mục đã bỏ qua trên lô di chuyển:</span><span class="sxs-lookup"><span data-stu-id="e5fbc-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="e5fbc-105">Sử dụng lệnh sau để phê duyệt các mục đã bỏ qua yêu cầu di chuyển "đồng bộ hóa" nhưng không hoàn thành:</span><span class="sxs-lookup"><span data-stu-id="e5fbc-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="e5fbc-106">Lô di chuyển và yêu cầu nên tiếp tục và hoàn thành trong vài phút.</span><span class="sxs-lookup"><span data-stu-id="e5fbc-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

