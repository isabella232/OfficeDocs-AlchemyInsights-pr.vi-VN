---
title: Khóa kích hoạt bỏ qua trên các thiết bị iOS được sử dụng với Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: de52ba77d3155d957372c31d465881fc7e8fcbbe657dfa35dedfee2be52e5a52
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046522"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Khóa kích hoạt bỏ qua trên các thiết bị iOS được sử dụng với Intune

Khả năng bỏ qua khóa kích hoạt trên thiết bị iOS sẽ giúp bạn dễ dàng phục hồi hơn từ kịch bản mà người dùng bật khóa kích hoạt trên thiết bị của công ty, rồi rời khỏi công ty.

Điều kiện tiên quyết để bỏ qua khóa kích hoạt bao gồm:

- Một thiết bị là "được hỗ trợ".
- Khóa kích hoạt được bật thành công bằng cách sử dụng chính sách hạn chế Thiết bị iOS trong Intune.

Ngoài ra, khi bỏ qua khóa kích hoạt, bạn nên:

- Về mặt vật lý, sở hữu thiết bị bị xóa.
- Sao chép mã trước khi thực hiện xóa.

**Lưu ý:** Mã xóa không nhạy cảm chữ hoa/thường, vì vậy không bắt buộc dùng ký tự "-".

Để biết chi tiết, [hãy xem Bỏ qua Khóa Kích hoạt trên thiết bị iOS đã sử dụng với Intune.](https://docs.microsoft.com/intune/device-activation-lock-bypass)

**Câu hỏi thường gặp**

Hỏi: Tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị, và bây giờ nó đang **kẹt ở trạng thái đang chờ xử lý.**

Đáp: Để hoàn tất thành công hành động từ xa, thiết bị mục tiêu phải trực tuyến và hoạt động tốt. Trong các tình huống sau, hành động từ xa nằm ở trạng thái chờ xử lý trong 30 ngày hoặc cho đến khi thiết bị xác nhận lệnh khi thiết bị:

- Không có kết nối.
- Mất trạng thái quản lý của nó với Intune.

Nếu bạn cho rằng thiết bị không còn kiểm nhập và thiết bị đó sẽ không loại bỏ dữ liệu công ty, hãy chọn Xóa. Việc xóa sẽ loại bỏ bản ghi thiết bị để bản ghi không còn xuất hiện trong danh sách thiết bị Intune. Để thiết bị hoạt động trở lại, người dùng của thiết bị phải đăng ký lại thiết bị.

Hỏi: Tại **sao một số hành động từ xa nhất định không sẵn dùng để tôi dùng?**

A: Không phải tất cả các nền tảng đều hỗ trợ tất cả các hành động của thiết bị từ xa. Các hành động từ xa sau đây dành riêng cho nền tảng.

- Bỏ qua Khóa Kích hoạt (chỉ iOS)
- Bắt đầu Từ đầu (Windows riêng)
- Chế độ bị mất (chỉ iOS)
- Định vị thiết bị (chỉ iOS)
- Khởi động lại (Windows lại)

Để biết thêm chi tiết về từng hành động, hãy xem Hành [động thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).