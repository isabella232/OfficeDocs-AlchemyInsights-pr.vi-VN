---
title: Sự cố với việc loại bỏ thiết bị bị xóa khỏi hoặc không còn sử dụng khỏi Hàng tồn kho Thiết bị
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324466"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Sự cố với việc loại bỏ thiết bị bị xóa khỏi hoặc không còn sử dụng khỏi Hàng tồn kho Thiết bị

Bộ bảo vệ Microsoft cho Điểm cuối hiện không cho phép loại bỏ theo cách thủ công bản ghi thiết bị của một thiết bị đã xóa khỏi hoặc ngừng hoạt động khỏi Kiểm kê Thiết bị.

Vì mục đích bảo mật, thiết bị vẫn ở trong cổng thông tin dưới dạng bản ghi lịch sử trong tối đa 180 ngày. Tuy nhiên, dữ liệu thiết bị sẽ được dọn sạch theo thời gian lưu giữ đã đặt cấu hình của bạn.

**Lưu ý:** Thiết bị đã xóa khỏi hoặc ngừng hoạt động sẽ tự động chuyển sang trạng **thái Không** hoạt động sau bảy ngày. Ngoài ra, thiết bị không hoạt động trong 30 ngày qua không được tính vào dữ liệu phản ánh điểm tiếp cận của tổ chức bạn Quản lý Mối đe dọa và Lỗ hổng điểm tiếp cận bảo mật của Microsoft dành cho thiết bị.
 
Nếu bạn vẫn không muốn thấy một số thiết bị trong chế độ xem Kiểm kê thiết bị, hãy thử đặt thẻ thiết bị để lọc thiết bị không hoạt động từ chế độ xem Kiểm kê Thiết bị.

Để biết thêm thông tin, hãy xem:

[Các thiết bị ngoài bảng từ Bộ bảo vệ Microsoft dành cho dịch vụ Điểm cuối](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Điểm phơi sáng trong Quản lý Mối đe dọa và Lỗ hổng](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Khắc phục các cảm biến không tốt trong Bộ bảo vệ Microsoft dành cho Điểm cuối](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cách sử dụng gắn thẻ hiệu quả (Phần 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cách sử dụng gắn thẻ hiệu quả (Phần 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cách sử dụng gắn thẻ hiệu quả (Phần 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




