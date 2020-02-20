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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158552"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="1e8d2-102">Khôi phục thư mục công cộng đã xóa</span><span class="sxs-lookup"><span data-stu-id="1e8d2-102">Restore a deleted public folder</span></span>

<span data-ttu-id="1e8d2-103">**Để khôi phục các mục đã xóa từ thư mục công cộng**:</span><span class="sxs-lookup"><span data-stu-id="1e8d2-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="1e8d2-104">Xem [bạn không thể khôi phục các mục đã xóa từ thư mục công cộng không thư trong Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="1e8d2-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="1e8d2-105">**Để khôi phục thư mục công cộng đã bị xóa (của bất kỳ loại nào)**:</span><span class="sxs-lookup"><span data-stu-id="1e8d2-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="1e8d2-106">Vui lòng sử dụng lệnh EXO PowerShell sau:</span><span class="sxs-lookup"><span data-stu-id="1e8d2-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="1e8d2-107">Cú pháp:</span><span class="sxs-lookup"><span data-stu-id="1e8d2-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="1e8d2-108">Ví dụ: lệnh sau sẽ khôi phục Subfolder1 và nơi nó dưới \Parent1:</span><span class="sxs-lookup"><span data-stu-id="1e8d2-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="1e8d2-109">Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="1e8d2-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
