---
title: Bỏ qua khóa kích hoạt trên các thiết bị iOS giám sát bằng InTune
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
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757322"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bỏ qua khóa kích hoạt trên các thiết bị iOS giám sát bằng InTune

Khả năng bỏ qua khóa kích hoạt trên thiết bị iOS giúp bạn phục hồi dễ dàng hơn từ tình huống mà người dùng bật khóa kích hoạt trên thiết bị công ty, rồi rời khỏi công ty.

Các site Pre-requiđể bỏ qua khóa kích hoạt bao gồm:

- Thiết bị là "có giám sát".
- Khóa kích hoạt đã được kích hoạt thành công bằng cách sử dụng chính sách hạn chế thiết bị iOS trong InTune.

Ngoài ra, khi bỏ qua khóa kích hoạt, bạn nên:

- Thể chất có thiết bị bị xóa sổ.
- Sao chép mã trước khi bạn phát hành xóa.

**Lưu ý:** Mã xóa không phân biệt chữ hoa/thường, vì vậy các ký tự "-" không bắt buộc.

Để biết chi tiết, hãy xem [bỏ qua khóa kích hoạt trên các thiết bị iOS có giám sát với InTune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**DIỄN**

Hỏi: **tôi đã ban hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị và bây giờ nó bị kẹt trong trạng thái đang chờ xử lý.**

A: đối với hành động từ xa để hoàn thành thành công, thiết bị đích phải trực tuyến và khỏe mạnh. Trong những tình huống sau đây, hành động từ xa vẫn nằm trong trạng thái đang chờ 30 ngày hoặc cho đến khi thiết bị thừa nhận lệnh khi thiết bị:

- Không có kết nối.
- Mất trạng thái quản lý của nó bằng InTune.

Nếu bạn cho rằng thiết bị không còn được kiểm tra và nó sẽ không loại bỏ dữ liệu công ty, hãy chọn xóa bỏ. Việc xóa bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách các thiết bị InTune. Đối với thiết bị hoạt động trở lại, người dùng của nó phải đăng ký lại thiết bị.

Hỏi: **tại sao những hành động từ xa nhất định không sẵn dùng cho tôi để sử dụng?**

A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa. Các hành động từ xa sau đây là nền tảng cụ thể.

- Bỏ qua khóa kích hoạt (chỉ dành cho iOS)
- Bắt đầu mới (chỉ dành cho Windows)
- Chế độ bị mất (chỉ dành cho iOS)
- Định vị thiết bị (chỉ dành cho iOS)
- Khởi động lại (chỉ dành cho Windows)

Để biết thêm chi tiết về từng hành động, hãy xem các [hành động của thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).