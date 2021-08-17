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
ms.openlocfilehash: 6eb59d16a1dab2de0e7a44faf9b34be6432342f9e20c94b6932e69e937751add
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892025"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>Sự cố với việc loại bỏ thiết bị bị xóa khỏi hoặc không còn sử dụng khỏi Hàng tồn kho Thiết bị

Bộ bảo vệ Microsoft cho Điểm cuối hiện không cho phép loại bỏ theo cách thủ công bản ghi thiết bị của một thiết bị đã xóa khỏi hoặc ngừng hoạt động khỏi Kiểm kê Thiết bị.

Vì mục đích bảo mật, thiết bị vẫn ở trong cổng thông tin dưới dạng bản ghi lịch sử trong tối đa 180 ngày. Tuy nhiên, dữ liệu thiết bị sẽ được dọn sạch theo thời gian lưu giữ đã đặt cấu hình của bạn.

**Lưu ý:** Thiết bị đã xóa khỏi hoặc ngừng hoạt động sẽ tự động chuyển sang trạng **thái Không** hoạt động sau bảy ngày. Ngoài ra, các thiết bị không hoạt động trong 30 ngày qua sẽ không được tính vào dữ liệu phản ánh điểm tiếp xúc Quản lý Mối đe dọa và Lỗ hổng của tổ chức bạn hoặc Điểm Số Bảo mật của Microsoft dành cho thiết bị.
 
Nếu bạn vẫn không muốn thấy một số thiết bị trong chế độ xem Kiểm kê thiết bị, hãy thử đặt thẻ thiết bị để lọc thiết bị không hoạt động từ chế độ xem Kiểm kê Thiết bị.

Để biết thêm thông tin, hãy xem:

[Các thiết bị ngoài bảng từ Bộ bảo vệ Microsoft dành cho dịch vụ Điểm cuối](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[Điểm phơi sáng trong Quản lý Mối đe dọa và Lỗ hổng](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Khắc phục các cảm biến không tốt trong Bộ bảo vệ Microsoft dành cho Điểm cuối](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[Cách sử dụng gắn thẻ hiệu quả (Phần 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[Cách sử dụng gắn thẻ hiệu quả (Phần 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[Cách sử dụng gắn thẻ hiệu quả (Phần 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




