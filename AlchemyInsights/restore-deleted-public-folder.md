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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="045e6-102">Khôi phục thư mục công cộng đã xóa</span><span class="sxs-lookup"><span data-stu-id="045e6-102">Restore a deleted public folder</span></span>

<span data-ttu-id="045e6-103">**Để khôi phục các mục đã xóa từ thư mục công cộng**:</span><span class="sxs-lookup"><span data-stu-id="045e6-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="045e6-104">Xem [bạn không thể khôi phục các mục đã xóa từ thư mục công cộng không thư trong Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="045e6-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="045e6-105">**Để khôi phục thư mục công cộng đã bị xóa (của bất kỳ loại nào)**:</span><span class="sxs-lookup"><span data-stu-id="045e6-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="045e6-106">Vui lòng sử dụng lệnh EXO PowerShell sau:</span><span class="sxs-lookup"><span data-stu-id="045e6-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="045e6-107">Cú pháp:</span><span class="sxs-lookup"><span data-stu-id="045e6-107">Syntax:</span></span>

    ><span data-ttu-id="045e6-108">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Tên-EQ "\<name_of_deleted_public_Folder"}; Set-PublicFolder $pf. Identity- \<đường dẫn nơi thư mục sẽ được khôi phục></span><span class="sxs-lookup"><span data-stu-id="045e6-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="045e6-109">Ví dụ: lệnh sau sẽ khôi phục Subfolder1 và nơi nó dưới \Parent1:</span><span class="sxs-lookup"><span data-stu-id="045e6-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="045e6-110">$pf = Get-PublicFolder \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-recurse |? {$_. Tên-EQ "Subfolder1"}; Thiết lập PublicFolder $pf. Identity-đường dẫn \Parent1</span><span class="sxs-lookup"><span data-stu-id="045e6-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="045e6-111">Xem [khôi phục thư mục công cộng đã xóa](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="045e6-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
