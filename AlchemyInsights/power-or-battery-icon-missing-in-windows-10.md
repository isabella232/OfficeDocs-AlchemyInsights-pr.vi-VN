---
title: Mất điện hoặc biểu tượng pin trong Windows 10
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
- "9002953"
- "5655"
ms.openlocfilehash: 10213843f8ec5ceeaa191d3373406d767f2bea3c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771563"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a>Mất điện hoặc biểu tượng pin trong Windows 10

Nếu thiết bị chạy Windows 10 của bạn có pin (ví dụ, máy tính xách tay hoặc máy tính bảng hoặc PC được kết nối qua cổng USB đến một UPS), thường là biểu tượng Power/Battery được hiển thị trong thanh tác vụ gần đồng hồ, ví dụ:

![Biểu tượng pin](media/battery-icon.png)

Nếu bạn không nhìn thấy biểu tượng này, có thể bạn sẽ bị ẩn:

1. Đi đến **[cài đặt > thanh tác vụ > cá](ms-settings:taskbar?activationSource=GetHelp)** nhân hóa.

2. Trong khu vực thông báo, hãy bấm **chọn biểu tượng nào xuất hiện trên thanh tác vụ**.

3. Sau đó tìm mục **Power** trong danh sách và chuyển đổi thiết đặt thành **bật**.

    ![Hiển thị biểu tượng Power trong thanh tác vụ](media/power-icon-on.png)

**Giải**

Nếu bạn đã làm theo các hướng dẫn trên và bật tắt của **Power** sẽ bị mờ đi hoặc không nhìn thấy được, trong hộp tìm kiếm trên thanh tác vụ, hãy nhập **trình quản lý thiết bị**, rồi chọn **Device Manager** trong danh sách kết quả. Bên dưới **pin**, bấm chuột phải vào pin cho thiết bị của bạn, bấm vào **tắt**, rồi bấm **có**. Chờ vài giây, rồi bấm chuột phải vào pin và bấm **bật**. Sau đó khởi động lại thiết bị của bạn.

Nếu bạn đã làm theo các hướng dẫn ở trên, nhưng biểu tượng pin không xuất hiện trên thanh tác vụ, trong hộp tìm kiếm trên thanh tác vụ, hãy gõ **trình quản lý tác vụ**, rồi bấm **trình quản lý tác vụ** trong danh sách kết quả. Trên tab **tiến trình** , bên dưới **tên**, hãy bấm chuột phải vào **Explorer**, rồi bấm vào **khởi động lại**.
