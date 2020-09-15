---
title: Chính sách chia sẻ trong lịch 618
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684252"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Lỗi chính sách khi chia sẻ lịch

1. Hãy thực hiện một trong những thao tác sau đây, phù hợp với tình huống của bạn:
    - Kết nối với Exchange Online bằng cách sử dụng Remote PowerShell. Để biết thêm thông tin, hãy xem [kết nối với Exchange Online bằng PowerShell từ xa](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Trên máy chủ tại cơ sở, hãy mở Exchange Management Shell.
2. Xác định chính sách chia sẻ được gán cho người dùng. Để thực hiện điều này, hãy chạy lệnh sau đây và ghi lại chính sách trả về:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Cập Nhật chính sách chia sẻ cho người dùng. Caranya sebagai berikut:
    - Mở Trung tâm quản trị Exchange.
    - Bấm **tổ chức**, rồi bấm đúp vào chính sách được gán cho người dùng bên dưới **chia sẻ riêng lẻ**. Đây là chính sách đã được trả về trong bước 2.
    - Trên trang chia sẻ quy tắc, hãy chọn mức chia sẻ lịch mà bạn muốn cho phép bên dưới **xác định những thông tin bạn muốn chia sẻ**; bấm **lưu**.

Để biết thêm thông tin, hãy xem: ["chính sách không cho phép cấp quyền ở mức này cho một hoặc nhiều lỗi" người nhận (các) "khi người dùng cố gắng chia sẻ lịch](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
