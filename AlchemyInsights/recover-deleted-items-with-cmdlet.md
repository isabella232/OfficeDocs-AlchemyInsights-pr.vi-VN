---
title: Khôi phục các mục đã xóa với lệnh ghép ngắn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 86744d92a44096991079d1da3bdf4e95e58c55b7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493424"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="9caef-102">Khôi phục các mục đã xóa với lệnh ghép ngắn</span><span class="sxs-lookup"><span data-stu-id="9caef-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="9caef-103">Sử dụng lệnh ghép ngắn [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) để xem các mục đã xóa trong hộp thư.</span><span class="sxs-lookup"><span data-stu-id="9caef-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="9caef-104">Sau khi bạn tìm thấy các mục đã xoá, bạn sử dụng lệnh ghép ngắn [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) để khôi phục chúng.</span><span class="sxs-lookup"><span data-stu-id="9caef-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="9caef-105">Xem chi tiết đầy đủ trong [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="9caef-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="9caef-106">Bạn cần được gán vai trò xuất nhập hộp thư trước khi bạn có thể chạy lệnh này.</span><span class="sxs-lookup"><span data-stu-id="9caef-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="9caef-107">Vui lòng xem [Get-RecoverableItems để](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="9caef-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
