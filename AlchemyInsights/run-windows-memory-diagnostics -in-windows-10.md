---
title: Chạy Chẩn Windows bộ nhớ trong Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922593"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Chạy Chẩn Windows bộ nhớ trong Windows 10

Nếu Windows và các ứng dụng trên PC của bạn gặp sự cố, đông đặc hoặc hoạt động theo cách không ổn định thì bạn có thể gặp sự cố với bộ nhớ (RAM) của PC. Bạn có thể chạy Chẩn Windows nhớ Người dùng nội bộ để kiểm tra sự cố với RAM của PC.

Trong hộp tìm kiếm trên thanh tác vụ của bạn, nhập **chẩn đoán bộ** nhớ , sau đó chọn Windows chẩn đoán bộ **nhớ**. 

Để chạy chẩn đoán, PC cần khởi động lại. Bạn có tùy chọn khởi động lại ngay lập tức (vui lòng lưu công việc của bạn và đóng tài liệu và email đang mở trước) hoặc lên lịch chẩn đoán để chạy tự động vào lần khởi động lại PC tiếp theo:

![Windows Chẩn đoán Bộ nhớ](media/windows-memory-diagnostic.png)

Khi PC khởi động lại, Công cụ **Chẩn đoán Windows nhớ sẽ tự** động chạy. Trạng thái và tiến độ sẽ được hiển thị khi chẩn đoán chạy, đồng thời, bạn có tùy chọn hủy bỏ chẩn đoán bằng cách nhấn phím **ESC** trên bàn phím.

Khi các chẩn đoán đã hoàn tất, các Windows sẽ bắt đầu bình thường.
Ngay sau khi khởi động lại, khi Màn hình  nền xuất hiện, một thông báo sẽ xuất hiện (cạnh biểu tượng Trung tâm Hành động trên thanh tác vụ), để cho biết có tìm thấy bất kỳ lỗi bộ nhớ nào không. Ví dụ:

Đây là biểu tượng Trung tâm Hành động: ![Biểu tượng Trung tâm hành động](media/action-center-icon.png) 

Và thông báo mẫu: ![Không có lỗi bộ nhớ](media/no-memory-errors.png)

Nếu bạn bỏ lỡ thông  báo, bạn có thể chọn  biểu tượng Trung tâm Hành động trên thanh tác vụ để hiển thị Trung tâm Hành động và xem danh sách thông báo có thể cuộn.

Để xem lại thông tin chi tiết, **hãy** nhập sự kiện vào hộp tìm kiếm trên thanh tác vụ của bạn, rồi chọn Trình **xem Sự kiện.** Trong ngăn **bên trái của Trình** xem Sự kiện, dẫn hướng tới Phần Windows Nhật ký > hệ **thống**. Trong ngăn bên phải, quét danh sách  trong khi đang xem cột Nguồn, cho đến khi bạn thấy các sự kiện với giá trị Source **MemoryDiagnostics-Results**. Tô sáng từng sự kiện đó và xem thông tin kết quả trong hộp bên **dưới** tab Chung bên dưới danh sách.
