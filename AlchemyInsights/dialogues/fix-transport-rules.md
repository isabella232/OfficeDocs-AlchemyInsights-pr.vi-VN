---
title: Sửa quy tắc truyền dẫn
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695867"
---
# <a name="fix-transport-rules"></a>Sửa quy tắc truyền dẫn

Quy tắc dòng thư tùy chỉnh ảnh hưởng đến thư này. Để xem lại quy tắc chính xác, hãy thực hiện như sau:

1. Trong kết quả nộp, bên dưới **thông tin bổ sung**, hãy lưu ý **GUID** hoặc **tên chính sách**.
2. Khởi động Exchange Management Shell. Để biết thêm thông tin, hãy xem [mở Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Chạy lệnh này (sử dụng GUID từ trình gửi của bạn):  **Get-TransportRule-Identity "GUID" | FL * mô tả***
4. Xem lại mô tả để xem các điều kiện được cấu hình ảnh hưởng đến thư.

Để tìm hiểu thêm, hãy xem [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
