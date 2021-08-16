---
title: Tìm hiểu xem ai thiết lập chuyển tiếp trên hộp thư và cách thức
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988255"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Tìm hiểu xem ai thiết lập chuyển tiếp trên hộp thư và cách thức

Nếu chuyển tiếp bên ngoài được đặt trên một hộp thư, hoạt động đó sẽ được kiểm tra như một phần của lệnh ghép Set-Mailbox ngắn. Sau đây là cách tìm hoạt động trong nhật ký kiểm tra:

1. Đi đến Trung [tâm Office 365 chính sách Bảo & Tuân thủ](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Chọn Tìm **kiếm Tìm** kiếm Nhật ký >  **kiểm tra**.
    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể lấy dữ liệu từ ngày trước đó.
1. Đảm bảo rằng trường **Hoạt** động được đặt thành Hiển **thị kết quả cho tất cả các hoạt** động (mặc định). Xác định phạm vi ngày. Bạn không cần chỉ định tên người dùng.
1. Chọn **Tìm kiếm**. Các hoạt động xuất hiện bên dưới **Kết quả**.
1. Chọn **Lọc Kết quả**, rồi nhập **Set-mailbox** vào trường **bộ lọc** Hoạt động. Thao tác này trả về **tất cả các hoạt động Set-Mailbox.**
1. Để xem chi tiết, hãy chọn một hoạt động, rồi chọn Xem **thêm Thông tin**. Bên **dưới Tham** số, bạn có thể thấy địa chỉ email chuyển tiếp đã được đặt trên hộp thư. **UserID đại diện** cho người dùng thiết lập chuyển tiếp bên ngoài trên hộp thư.
Để tìm hiểu thêm, xem mục [Tìm kiếm nhật Office 365 kiểm tra để khắc phục các tình huống phổ biến.](https://go.microsoft.com/fwlink/?linkid=2103944)