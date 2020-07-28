---
title: Định vị các thiết bị iOS bị mất với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440434"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Định vị các thiết bị iOS bị mất với InTune

Cho phép chế độ mất trên thiết bị iOS cho phép quản trị viên có thư và số điện thoại liên hệ được hiển thị trên màn hình khóa.

Sau khi chế độ bị mất được kích hoạt quản trị viên có thể sử dụng định vị hành động thiết bị để xác định vị trí vật lý của thiết bị.

Hành động xác định thiết bị trong InTune hoạt động với thiết bị iOS để hiển thị vị trí của một thiết bị cụ thể trên bản đồ.

Sử dụng hành động này yêu cầu thiết bị iOS được trong:

- Chế độ giám sát
- Chế độ mất

Để biết thêm thông tin, hãy xem [bật chế độ mất trên các thiết bị iOS/iPadOS với InTune](https://docs.microsoft.com/intune/device-lost-mode) và [định vị các thiết bị bị mất hoặc đánh cắp iOS/ipados với InTune](https://docs.microsoft.com/intune/device-locate).

**Faq**

Câu hỏi: tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu của công ty khỏi thiết bị và bây giờ nó được dán ở trạng thái chờ.

A: đối với một hành động từ xa để hoàn thành thành công, các thiết bị mục tiêu phải trực tuyến và khỏe mạnh. Trong các trường hợp sau, hành động từ xa ở trạng thái chờ trong 30 ngày, hoặc cho đến khi thiết bị thừa công lệnh:

- Khi thiết bị không có kết nối
- Khi thiết bị mất trạng thái quản lý với InTune

Nếu bạn cho rằng thiết bị không còn được kiểm tra và không thể xóa dữ liệu công ty, hãy chọn xóa. Xóa loại bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách thiết bị InTune. Nếu thiết bị trở nên hoạt động trở lại, người dùng của nó sẽ phải đăng ký lại nó.

Hỏi: tại sao một số hành động từ xa không có sẵn cho tôi để sử dụng?

A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa. Các hành động từ xa sau đây là nền tảng cụ thể, vì vậy chúng chỉ có sẵn cho các nền tảng được ghi nhận.

- Khóa kích hoạt bỏ qua (chỉ iOS)
- Khởi động mới (chỉ dành cho Windows)
- Chế độ mất (chỉ iOS)
- Xác định vị trí thiết bị (iOS chỉ)
- Khởi động lại (chỉ dành cho Windows)

Để biết thêm chi tiết về từng hành động, xem [hành động của thiết bị có sẵn](https://docs.microsoft.com/intune/device-management#available-device-actions).