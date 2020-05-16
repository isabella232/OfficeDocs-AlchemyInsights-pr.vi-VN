---
title: Nguồn điện hoặc biểu tượng pin bị thiếu trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: d82994c86126ea9c789e846a74e03794c32c5c3c
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44269521"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Nguồn điện hoặc biểu tượng pin bị thiếu trong Windows 10

Nếu thiết bị chạy Windows 10 của bạn có pin (ví dụ: máy tính xách tay hoặc máy tính bảng hoặc PC kết nối qua USB với một UPS), thông thường một biểu tượng nguồn/pin được hiển thị trong thanh tác vụ gần đồng hồ, ví dụ:

![Biểu tượng pin](media/battery-icon.png)

Nếu bạn không thấy biểu tượng này, nó có thể bị ẩn:

1. Đi tới **[cài đặt > cá nhân hóa > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.

2. Trong khu vực thông báo, bấm **chọn các biểu tượng xuất hiện trên thanh tác vụ**.

3. Sau đó tìm mục **Power** trong danh sách và chuyển đổi cài đặt của nó thành **bật**.

    ![Hiển thị biểu tượng nguồn điện trong thanh tác vụ](media/power-icon-on.png)

**Troubleshooting**

Nếu bạn đã làm theo các hướng dẫn ở trên và bật tắt **nguồn** màu xám hoặc không hiển thị, trong hộp tìm kiếm trên thanh tác vụ, hãy nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** trong danh sách kết quả. Trong **pin**, bấm chuột phải vào pin cho thiết bị của bạn, bấm **vô hiệu hoá**và bấm **có**. Chờ một vài giây, và sau đó nhấp chuột phải vào pin và **kích hoạt**. Sau đó khởi động lại thiết bị của bạn.

Nếu bạn làm theo các hướng dẫn ở trên, nhưng biểu tượng pin không xuất hiện trên thanh tác vụ, trong hộp tìm kiếm trên thanh tác vụ, gõ **Task Manager**, và sau đó nhấp vào **Task Manager** trong danh sách kết quả. Trên tab **quy trình** , trong **tên**, bấm chuột phải vào **Explorer**, và sau đó bấm **khởi động lại**.
