---
title: Xác định vị trí các thiết bị iOS bị mất với Intune
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
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042328"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Xác định vị trí các thiết bị iOS bị mất với Intune

Bật chế độ mất trên thiết bị iOS cho phép người quản trị hiển thị tin nhắn và số điện thoại liên hệ trên màn hình khóa.

Sau khi chế độ bị mất được bật, người quản trị có thể sử dụng hành động Định vị thiết bị để xác định vị trí vật lý của thiết bị.

Hành động Định vị thiết bị trong Intune hoạt động với thiết bị iOS để hiển thị vị trí của một thiết bị cụ thể trên bản đồ.

Việc sử dụng hành động này đòi hỏi thiết bị iOS phải hoạt động:

- Chế độ có tổ hợp
- Chế độ bị mất

Để biết thêm thông tin, hãy xem mục Bật chế độ bị mất trên thiết bị [iOS/iPadOS với Intune](https://docs.microsoft.com/intune/device-lost-mode) và Xác định vị trí thiết bị [iOS/iPadOS](https://docs.microsoft.com/intune/device-locate)bị mất hoặc bị đánh cắp với Intune .

**Câu hỏi thường gặp**

Hỏi: Tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị, và bây giờ nó đang kẹt ở trạng thái đang chờ xử lý.

Đáp: Để hoàn tất thành công hành động từ xa, thiết bị mục tiêu phải trực tuyến và hoạt động tốt. Trong các tình huống sau, hành động từ xa nằm ở trạng thái chờ xử lý trong 30 ngày hoặc cho đến khi thiết bị chấp nhận lệnh:

- Khi thiết bị không có kết nối
- Khi thiết bị mất trạng thái quản lý với Intune

Nếu bạn cho rằng thiết bị không còn kiểm nhập và thiết bị đó sẽ không thể loại bỏ dữ liệu công ty, hãy chọn Xóa. Việc xóa sẽ loại bỏ bản ghi thiết bị để bản ghi không còn xuất hiện trong danh sách thiết bị Intune. Nếu thiết bị trở nên hiện hoạt lại, người dùng của thiết bị sẽ phải đăng ký lại thiết bị.

Hỏi: Tại sao một số hành động từ xa nhất định không sẵn dùng để tôi dùng?

A: Không phải tất cả các nền tảng đều hỗ trợ tất cả các hành động của thiết bị từ xa. Các hành động từ xa sau đây dành riêng cho nền tảng, vì vậy chúng chỉ sẵn dùng cho những nền tảng được chú ý.

- Bỏ qua Khóa Kích hoạt (chỉ iOS)
- Bắt đầu Từ đầu (Windows riêng)
- Chế độ bị mất (chỉ iOS)
- Định vị thiết bị (chỉ iOS)
- Khởi động lại (Windows lại)

Để biết thêm chi tiết về từng hành động, hãy xem Hành [động thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).