---
title: Chính sách Chia sẻ Lịch 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091631"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Lỗi chính sách khi chia sẻ lịch

1. Thực hiện một trong những cách sau đây, phù hợp với tình huống của bạn:
    - Kết nối cập Exchange Online cách sử dụng Remote PowerShell. Để biết thêm thông tin, [hãy xem Kết nối tìm Exchange Online cách sử dụng Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Trên máy chủ tại chỗ, hãy mở trình Exchange Management Shell.
2. Xác định chính sách chia sẻ được gán cho người dùng. Để thực hiện điều này, hãy chạy lệnh sau đây và ghi chú chính sách được trả về:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Cập nhật chính sách chia sẻ cho người dùng. Caranya sebagai berikut:
    - Mở trung tâm quản Exchange chính.
    - Bấm **Tổ** chức , rồi bấm đúp vào chính sách được gán cho người dùng bên dưới Chia **sẻ Cá nhân.** Đây là chính sách được trả về ở bước 2.
    - Trên trang Quy tắc Chia sẻ, hãy chọn mức chia sẻ lịch mà bạn muốn cho phép trong Xác **định những thông tin bạn muốn chia sẻ**; bấm **Lưu**.

Để biết thêm thông tin, hãy xem mục: Lỗi "Chính sách không cho phép cấp quyền ở cấp độ này cho một hoặc nhiều người nhận" khi người dùng tìm cách [chia sẻ lịch.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
