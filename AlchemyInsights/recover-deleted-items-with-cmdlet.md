---
title: Khôi phục các mục đã xóa bằng lệnh ghép ngắn
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: b3f4f034d5d7486dafa1b5c1801a285b09a34644b811146f09f454fad9647833
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910676"
---
# <a name="recover-deleted-items-with-cmdlet"></a>Khôi phục các mục đã xóa bằng lệnh ghép ngắn

- Sử dụng [lệnh ghép ngắn Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) để xem các mục đã xóa trong hộp thư. Sau khi tìm thấy các mục đã xóa, bạn hãy sử dụng lệnh ghép ngắn [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) để khôi phục các mục đó.

- Xem chi tiết đầy đủ [trong Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).

- Bạn cần được gán vai trò Nhập Xuất Hộp thư trước khi có thể chạy lệnh ghép ngắn này. Vui lòng xem [Get-RecoverableItems để](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) biết thêm thông tin.
