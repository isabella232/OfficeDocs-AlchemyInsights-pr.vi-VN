---
title: Khắc phục quy tắc truyền tải
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034776"
---
# <a name="fix-transport-rules"></a>Khắc phục quy tắc truyền tải

Quy tắc dòng thư tùy chỉnh đã ảnh hưởng đến thư này. Để xem lại quy tắc chính xác, hãy làm như sau:

1. Trong kết quả gửi đi, bên **dưới Thông tin bổ** sung, ghi lại **GUID** hoặc **Tên Chính sách**.
2. Khởi Exchange Management Shell. Để biết thêm thông tin, [hãy xem Mở Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Chạy lệnh này (sử dụng GUID từ bài gửi của  **bạn): Get-TransportRule -identity "GUID" | fl * Description***
4. Xem lại mô tả để xem các điều kiện cấu hình ảnh hưởng đến thư.

Để tìm hiểu thêm, [hãy xem Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
