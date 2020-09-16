---
title: Khôi phục các mục đã xóa với lệnh ghép ngắn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741341"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="45a34-102">Khôi phục các mục đã xóa với lệnh ghép ngắn</span><span class="sxs-lookup"><span data-stu-id="45a34-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="45a34-103">Sử dụng lệnh ghép ngắn [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) để xem các mục đã xóa trong hộp thư.</span><span class="sxs-lookup"><span data-stu-id="45a34-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="45a34-104">Sau khi bạn tìm thấy các mục đã xóa, bạn sử dụng lệnh ghép ngắn [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) để khôi phục chúng.</span><span class="sxs-lookup"><span data-stu-id="45a34-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="45a34-105">Xem chi tiết đầy đủ trong [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="45a34-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="45a34-106">Bạn cần được gán vai trò xuất nhập hộp thư trước khi bạn có thể chạy lệnh ghép ngắn này.</span><span class="sxs-lookup"><span data-stu-id="45a34-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="45a34-107">Vui lòng xem [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="45a34-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
