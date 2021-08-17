---
title: Trạng thái cảm biến kiểm tra điểm cuối của Bộ bảo vệ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: cefebe63e45caab176ba84a35280378ace7e6b3115c48694ed043a39b4d93c1e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890076"
---
# <a name="defender-endpoint-check-sensor-status"></a>Trạng thái cảm biến kiểm tra điểm cuối của Bộ bảo vệ

Lát **xếp Thiết bị có sự cố cảm** biến nằm trên bảng điều khiển Hoạt động Bảo mật. Ô xếp này cung cấp thông tin về khả năng cung cấp dữ liệu cảm biến và liên lạc với Bộ bảo vệ cho dịch vụ Điểm cuối của thiết bị riêng lẻ. Tài liệu này báo cáo số lượng thiết bị cần chú ý và giúp bạn xác định các thiết bị gặp sự cố và thực hiện hành động để khắc phục các sự cố đã biết.

Hai chỉ báo trạng thái trên lát xếp cung cấp thông tin về số lượng thiết bị không báo cáo đúng cách với dịch vụ:

- **Đã cấu hình sai** Các thiết bị có thể báo cáo một phần dữ liệu cảm biến tới Bộ bảo vệ dành cho dịch vụ Điểm cuối và có thể gặp các lỗi về cấu hình cần sửa.
- **Không hoạt động** Các thiết bị đã ngừng báo cáo cho Bộ bảo vệ dành cho dịch vụ Điểm cuối trong hơn bảy ngày trong tháng trước.

Bấm vào bất kỳ nhóm nào sẽ hướng bạn đến danh sách Thiết bị, được lọc theo lựa chọn của bạn. Trên danh sách Thiết bị, bạn có thể lọc danh sách trạng thái theo trạng thái sau đây:

- **Hiện hoạt** Các thiết bị đang tích cực báo cáo cho Bộ bảo vệ dành cho dịch vụ Điểm cuối.
- **Đã cấu hình sai** Các thiết bị có thể báo cáo một phần dữ liệu cảm biến tới Bộ bảo vệ dành cho dịch vụ Điểm cuối nhưng gặp các lỗi về cấu hình cần được sửa. Thiết bị bị cấu hình sai có thể có một hoặc một sự cố kết hợp các vấn đề sau đây:

    - Không có dữ liệu cảm biến - Thiết bị đã ngừng gửi dữ liệu cảm biến. Có thể kích hoạt cảnh báo hạn chế từ thiết bị.
    - Giao tiếp bị khiếm khuyết - Khả năng giao tiếp với thiết bị suy giảm. Gửi tệp để phân tích chuyên sâu, chặn tệp, cách ly thiết bị khỏi mạng và các hành động khác yêu cầu liên lạc với thiết bị có thể không hoạt động.
- **Không hoạt động** Các thiết bị đã ngừng báo cáo với Bộ bảo vệ dành cho dịch vụ Điểm cuối.

Bạn có thể tải xuống toàn bộ danh sách ở định dạng CSV bằng cách sử dụng tính năng Xuất.

Để biết thêm thông tin, xem [mục Kiểm tra trạng thái cảm biến trong Bộ bảo vệ Microsoft dành cho Điểm cuối](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/check-sensor-status).

Để biết thêm thông tin về nguyên nhân thiết bị không hoạt động hoặc cấu hình sai, xem mục Khắc phục các cảm biến không tốt trong Bộ bảo [vệ Microsoft dành](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)cho Điểm cuối .
