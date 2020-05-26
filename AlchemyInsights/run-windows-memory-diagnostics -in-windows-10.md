---
title: Chạy Windows chẩn đoán bộ nhớ trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358289"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Chạy Windows chẩn đoán bộ nhớ trong Windows 10

Nếu Windows và các ứng dụng trên máy tính của bạn bị rơi, đóng băng hoặc hành động một cách không ổn định, bạn có thể gặp sự cố với bộ nhớ (RAM) của PC. Bạn có thể chạy các chẩn đoán bộ nhớ Windows để kiểm tra các vấn đề với RAM của máy tính.

Trong hộp tìm kiếm trên thanh tác vụ của bạn, hãy nhập **chẩn đoán bộ nhớ**, sau đó chọn **chẩn đoán bộ nhớ Windows**. 

Để chạy chẩn đoán, máy tính cần khởi động lại. Bạn có tùy chọn để khởi động lại ngay lập tức (Hãy lưu công việc của bạn và đóng tài liệu mở và e-mail đầu tiên), hoặc lịch trình chẩn đoán để chạy tự động trong lần tiếp theo máy tính khởi động lại:

![Chẩn đoán bộ nhớ Windows](media/windows-memory-diagnostic.png)

Khi máy tính khởi động lại, **công cụ chẩn đoán bộ nhớ của Windows** sẽ tự chạy. Trạng thái và tiến trình sẽ được hiển thị khi chạy chẩn đoán và bạn có tùy chọn hủy chẩn đoán bằng việc nhấn phím **esc** trên bàn phím.

Khi chẩn đoán hoàn tất, Windows sẽ bắt đầu bình thường.
Ngay sau khi khởi động lại, khi máy tính để bàn xuất hiện, một thông báo sẽ xuất hiện (bên cạnh biểu tượng **Trung tâm hành động** trên thanh tác vụ), để cho biết bất kỳ lỗi bộ nhớ nào được tìm thấy. Ví dụ:

Dưới đây là biểu tượng Action Center: ![Biểu tượng Trung tâm hành động](media/action-center-icon.png) 

Và một thông báo mẫu: ![Không có lỗi bộ nhớ](media/no-memory-errors.png)

Nếu bạn bỏ qua thông báo, bạn có thể chọn biểu tượng **Trung tâm hành động** trên thanh tác vụ để hiển thị **Trung tâm hành động** và xem danh sách thông báo có thể cuộn.

Để xem lại thông tin chi tiết, hãy nhập **sự kiện** vào hộp tìm kiếm trên thanh tác vụ của bạn, sau đó chọn trình chuyển đổi **sự kiện**. Trong ngăn bên trái của **trình xem sự kiện**, điều hướng đến **nhật ký Windows > hệ thống**. Trong ngăn bên phải, quét danh sách trong khi nhìn vào cột **nguồn** , cho đến khi bạn thấy sự kiện với nguồn giá trị **memorydiagnostics-kết quả**. Làm nổi bật mỗi sự kiện như vậy và xem thông tin kết quả trong hộp dưới tab **chung** bên dưới danh sách.
