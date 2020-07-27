---
title: Bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424285"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune

Khả năng bỏ qua khóa kích hoạt trên các thiết bị iOS giúp dễ dàng khôi phục từ tình huống mà người dùng cho phép khóa kích hoạt trên thiết bị công ty và sau đó rời khỏi công ty.

Pre-requisites để bỏ qua một khóa kích hoạt bao gồm:

- Một thiết bị là "được giám sát."
- Khóa kích hoạt được kích hoạt thành công bằng cách sử dụng chính sách hạn chế thiết bị iOS trong InTune.

Ngoài ra, khi bỏ qua một khóa kích hoạt, bạn nên:

- Thể chất có thiết bị bị xóa.
- Sao chép mã trước khi bạn phát hành xoá.

**Lưu ý:** Xoá mã không phải là trường hợp nhạy cảm, do đó, các ký tự "-" là không cần thiết.

Để biết chi tiết, xem [bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Faq**

Câu hỏi: **tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu của công ty khỏi thiết bị và bây giờ nó được dán ở trạng thái chờ.**

A: đối với một hành động từ xa để hoàn thành thành công, các thiết bị mục tiêu phải trực tuyến và khỏe mạnh. Trong các trường hợp sau, hành động từ xa ở trạng thái chờ trong 30 ngày, hoặc cho đến khi thiết bị thừa công lệnh khi thiết bị:

- Không có kết nối.
- Mất trạng thái quản lý của mình với InTune.

Nếu bạn cho rằng một thiết bị không còn kiểm tra và nó sẽ không xóa dữ liệu công ty, hãy chọn xóa. Xóa loại bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách thiết bị InTune. Để thiết bị hoạt động trở lại, người dùng phải đăng ký lại thiết bị.

Hỏi: **tại sao một số hành động từ xa không có sẵn cho tôi để sử dụng?**

A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa. Các hành động từ xa sau đây là nền tảng cụ thể.

- Khóa kích hoạt bỏ qua (chỉ iOS)
- Khởi động mới (chỉ dành cho Windows)
- Chế độ mất (chỉ iOS)
- Xác định vị trí thiết bị (iOS chỉ)
- Khởi động lại (chỉ dành cho Windows)

Để biết thêm chi tiết về từng hành động, xem [hành động của thiết bị có sẵn](https://docs.microsoft.com/intune/device-management#available-device-actions).