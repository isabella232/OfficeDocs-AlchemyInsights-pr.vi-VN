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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="eedb9-102">Thư mục công cộng lô di chuyển với trạng thái Completedwithlỗi</span><span class="sxs-lookup"><span data-stu-id="eedb9-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="eedb9-103">Sử dụng các bước sau để hoàn thành lô, bỏ qua các mục lớn/xấu:</span><span class="sxs-lookup"><span data-stu-id="eedb9-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="eedb9-104">Phê duyệt các mục đã bỏ qua trên lô di chuyển:</span><span class="sxs-lookup"><span data-stu-id="eedb9-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="eedb9-105">Thiết lập MigrationBatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="eedb9-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="eedb9-106">Sử dụng lệnh sau để phê duyệt các mục đã bỏ qua yêu cầu di chuyển "đồng bộ hóa" nhưng không hoàn thành:</span><span class="sxs-lookup"><span data-stu-id="eedb9-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="eedb9-107">$pf = Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics-IncludeReport; ForEach ($i trong $pf) {if ($i. LargeItemsEncountered-gt 0-hoặc $i. BadItemsEncountered-gt 0) {Set-PublicFolderMailboxMigrationRequest $i. Identity. IdentifyingGuid-SkippedItemApprovalTime $ ([DateTime]:: UtcNow)}}</span><span class="sxs-lookup"><span data-stu-id="eedb9-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="eedb9-108">Lô di chuyển và yêu cầu nên tiếp tục và hoàn thành trong vài phút.</span><span class="sxs-lookup"><span data-stu-id="eedb9-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

