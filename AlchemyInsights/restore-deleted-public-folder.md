---
title: Khôi phục thư mục công cộng đã xóa
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
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774553"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="129fc-102">Khôi phục thư mục công cộng đã xóa</span><span class="sxs-lookup"><span data-stu-id="129fc-102">Restore a deleted public folder</span></span>

<span data-ttu-id="129fc-103">**Để khôi phục các mục đã xóa khỏi thư mục công cộng**:</span><span class="sxs-lookup"><span data-stu-id="129fc-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="129fc-104">Xem [bạn không thể khôi phục các mục đã xóa khỏi thư mục công cộng không phải thư trong Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="129fc-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="129fc-105">**Để khôi phục thư mục công cộng đã xóa (trong bất kỳ loại nào)**:</span><span class="sxs-lookup"><span data-stu-id="129fc-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="129fc-106">Vui lòng dùng lệnh EXO PowerShell sau đây:</span><span class="sxs-lookup"><span data-stu-id="129fc-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="129fc-107">Syntax</span><span class="sxs-lookup"><span data-stu-id="129fc-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="129fc-108">Ví dụ: lệnh sau đây sẽ khôi phục Subfolder1 và đặt nó dưới \Parent1:</span><span class="sxs-lookup"><span data-stu-id="129fc-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="129fc-109">Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="129fc-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
