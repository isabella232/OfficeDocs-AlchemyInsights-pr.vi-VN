---
title: Tìm hiểu xem ai đã thiết lập chuyển tiếp trên hộp thư và cách thức
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430305"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Tìm hiểu xem ai đã thiết lập chuyển tiếp trên hộp thư và cách thức

Nếu việc chuyển tiếp bên ngoài được đặt trên một hộp thư, hoạt động được kiểm toán như là một phần của lệnh ghép ngắn Set-Mailbox. Sau đây là cách tìm kiếm hoạt động trong Nhật ký kiểm tra:

1. Đi đến [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Chọn **Tìm** >  **kiếm Nhật ký kiểm** tra.
    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật kiểm định, hãy tiếp tục và bật tính năng này ngay bây giờ. Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể kéo dữ liệu từ ngày trước đó.
1. Đảm bảo rằng trường **hoạt động** được thiết lập để **Hiển thị kết quả cho tất cả các hoạt động** (mặc định). Xác định phạm vi ngày. Bạn không cần phải xác định tên người dùng.
1. Chọn **Tìm kiếm**. Các hoạt động sẽ xuất hiện bên dưới **kết quả**.
1. Chọn **lọc kết quả**, rồi nhập **Set-Mailbox** trong trường bộ lọc **hoạt động** . Điều này trả về tất cả các hoạt động **đặt hộp thư** .
1. Để xem chi tiết, hãy chọn một hoạt động, rồi chọn **xem thêm thông tin**. Bên dưới **tham số** , bạn có thể thấy địa chỉ email chuyển tiếp đã được đặt trên hộp thư. **Userid** đại diện cho người dùng đã thiết lập việc chuyển tiếp bên ngoài trên hộp thư.
Để tìm hiểu thêm, hãy xem [Tìm kiếm Nhật ký kiểm tra Office 365 để khắc phục các kịch bản phổ biến](https://go.microsoft.com/fwlink/?linkid=2103944).