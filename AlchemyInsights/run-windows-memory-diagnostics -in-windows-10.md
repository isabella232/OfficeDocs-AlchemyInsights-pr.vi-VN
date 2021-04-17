---
title: Chạy chẩn đoán bộ nhớ Windows trong Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826689"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Chạy chẩn đoán bộ nhớ Windows trong Windows 10

Nếu Windows và ứng dụng trên PC của bạn bị rơi, đóng băng hoặc làm việc theo cách không ổn định, bạn có thể gặp phải sự cố với bộ nhớ của PC (RAM). Bạn có thể chạy chẩn đoán bộ nhớ Windows để kiểm tra các vấn đề với RAM của PC.

Trong hộp tìm kiếm trên thanh tác vụ, nhập **chẩn đoán bộ nhớ**, rồi chọn **chẩn đoán bộ nhớ Windows**. 

Để chạy chẩn đoán, PC cần phải khởi động lại. Bạn có tùy chọn khởi động lại ngay lập tức (vui lòng lưu công việc của bạn và đóng tài liệu mở và email đầu tiên) hoặc lên lịch chẩn đoán để chạy tự động lần sau khi PC khởi động lại:

![Chẩn đoán bộ nhớ Windows](media/windows-memory-diagnostic.png)

Khi PC khởi động lại, **công cụ chẩn đoán bộ nhớ Windows** sẽ chạy tự động. Trạng thái và tiến độ sẽ được hiển thị ở dạng chạy chẩn đoán và bạn có tùy chọn hủy bỏ chẩn đoán bằng cách nhấn phím **esc** trên bàn phím của bạn.

Khi chẩn đoán hoàn tất, Windows sẽ bắt đầu bình thường.
Ngay sau khi khởi động lại, khi máy tính của bạn xuất hiện, một thông báo sẽ xuất hiện (bên cạnh biểu tượng **Trung tâm hành động** trên thanh tác vụ), để cho biết liệu mọi lỗi đã tìm thấy bộ nhớ. Ví dụ:

Sau đây là biểu tượng Trung tâm hành động: ![Biểu tượng Trung tâm hành động](media/action-center-icon.png) 

Và thông báo mẫu: ![Không có lỗi bộ nhớ](media/no-memory-errors.png)

Nếu bạn bị nhỡ thông báo, bạn có thể chọn biểu tượng **Trung tâm hành động** trên thanh tác vụ để hiển thị **Trung tâm hành động** và xem danh sách thông báo có thể cuộn.

Để xem lại thông tin chi tiết, hãy nhập **sự kiện** vào hộp tìm kiếm trên thanh tác vụ của bạn, rồi chọn **trình xem sự kiện**. Trong ngăn bàn tay trái của **trình xem sự kiện**, dẫn hướng đến **hệ thống > Nhật ký** của bạn. Trong ngăn bên phải, hãy quét xuống danh sách trong khi đang xem cột **nguồn** , cho đến khi bạn thấy các sự kiện với **memorydiagnostics giá trị nguồn-kết quả**. Tô sáng từng sự kiện đó và xem thông tin kết quả trong hộp bên dưới tab **chung** bên dưới danh sách.
