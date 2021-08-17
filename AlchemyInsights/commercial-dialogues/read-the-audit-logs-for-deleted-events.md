---
title: Đọc nhật ký kiểm tra cho các sự kiện đã xóa
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
ms.openlocfilehash: ef4cbb0b778b22fba83d22d5056449c2281c5a2947ecb41ce8f808a4d1132426
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896037"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Đọc nhật ký kiểm tra cho các sự kiện đã xóa

Dưới đây là cách thực hiện:

1. Thực hiện một trong các thao tác sau:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật tính năng này, hãy tiếp tục và bật tính năng ngay bây giờ. Nếu tính năng này không bật, kết quả tìm kiếm sẽ không thể lấy dữ liệu từ ngày trước đó.

2. Trên tab Tìm **kiếm** của trang Kiểm **tra,** hãy cấu hình các thiết đặt sau:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt động**: Nhập **Exchange động trong hộp thư,** sau đó chọn các giá trị sau:
     - **Đã xóa thư khỏi thư mục Các mục Đã xóa**
     - **Đã di chuyển thư vào thư mục Các mục Đã xóa**

       Khi bạn thực hiện xong, hãy bấm vào bên ngoài ngăn để thu nhỏ ngăn **Hoạt** động.

   - **Người dùng:** Chấp nhận giá trị mặc định trống để trả về kết quả cho tất cả người dùng hoặc nhập một hoặc nhiều người dùng.

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Chọn một hoạt động trong kết quả để mở hộp bật lên chi tiết. Thông tin bổ sung về mục đã xóa, chẳng hạn như dòng chủ đề và vị trí của mục khi mục bị xóa, sẽ được hiển thị trong trường **Mục bị Ảnh** hưởng.

   > [!NOTE]
   > Bạn không thể khôi phục các mục đã xóa bằng tính năng nhật ký kiểm tra. Để khôi phục các mục đã xóa, [hãy xem Khôi phục email đã xóa Outlook trên web.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Để biết thêm thông tin, hãy xem [Tìm kiếm nhật ký kiểm tra để điều tra các sự cố hỗ trợ phổ biến.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
