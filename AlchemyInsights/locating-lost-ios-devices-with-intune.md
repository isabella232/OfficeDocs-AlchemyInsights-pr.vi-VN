---
title: Định vị mất thiết bị iOS với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675214"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Định vị mất thiết bị iOS với InTune

Bật chế độ bị mất trên thiết bị iOS cho phép người quản trị có thư và liên hệ với số điện thoại được hiển thị trên màn hình khóa.

Sau khi chế độ bị mất được bật người quản trị có thể sử dụng hành động định vị thiết bị để xác định vị trí thực của thiết bị.

Hành động định vị thiết bị trong InTune hoạt động với thiết bị iOS để hiển thị vị trí của một thiết bị cụ thể trên bản đồ.

Sử dụng hành động này yêu cầu thiết bị iOS được in:

- Chế độ giám sát
- Chế độ bị mất

Để biết thêm thông tin, hãy xem [bật chế độ bị mất trên thiết bị iOS/iPadOS có InTune](https://docs.microsoft.com/intune/device-lost-mode) và [xác định vị trí bị mất hoặc bị đánh cắp các thiết bị iOS/Ipados với InTune](https://docs.microsoft.com/intune/device-locate).

**DIỄN**

Hỏi: tôi đã ban hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị và bây giờ nó bị kẹt trong trạng thái đang chờ xử lý.

A: đối với hành động từ xa để hoàn thành thành công, thiết bị đích phải trực tuyến và khỏe mạnh. Trong những tình huống sau đây, hành động từ xa vẫn nằm trong trạng thái đang chờ 30 ngày hoặc cho đến khi thiết bị thừa nhận lệnh:

- Khi thiết bị không có kết nối
- Khi thiết bị mất trạng thái quản lý của nó bằng InTune

Nếu bạn cho rằng thiết bị không còn được kiểm tra tại đó, và nó sẽ không thể loại bỏ dữ liệu của công ty, chọn xóa. Việc xóa bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách các thiết bị InTune. Nếu thiết bị trở thành hoạt động trở lại, người dùng sẽ phải đăng ký lại nó.

Hỏi: tại sao những hành động từ xa nhất định không sẵn dùng cho tôi để sử dụng?

A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa. Các hành động từ xa sau đây là nền tảng cụ thể, do đó, chúng chỉ sẵn dùng cho những nền tảng được ghi chú.

- Bỏ qua khóa kích hoạt (chỉ dành cho iOS)
- Bắt đầu mới (chỉ dành cho Windows)
- Chế độ bị mất (chỉ dành cho iOS)
- Định vị thiết bị (chỉ dành cho iOS)
- Khởi động lại (chỉ dành cho Windows)

Để biết thêm chi tiết về từng hành động, hãy xem các [hành động của thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).