---
title: Tìm các sự kiện được thực hiện trên quy tắc hộp thư đến
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
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882657"
---
# <a name="find-events-performed-on-inbox-rules"></a>Tìm các sự kiện được thực hiện trên quy tắc hộp thư đến

Khi các quy tắc hộp thư đến được tạo, thay đổi hoặc xóa, các sự kiện được ghi lại trong nhật ký kiểm tra. Dưới đây là cách xem lại các thay đổi đó:

1. Thực hiện một trong các thao tác sau:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

    > [!NOTE]
    > Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể lấy dữ liệu từ ngày trước đó.

2. Trên tab Tìm **kiếm** của trang Kiểm **tra,** hãy cấu hình các thiết đặt sau:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt** động : Chọn **Quy tắc Hộp thư đến Mới Tạo quy tắc hộp thư đến từ Outlook Web App**

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Chọn một hoạt động trong kết quả để mở hộp bật lên chi tiết. Bên dưới **phần Tham** số, bạn có thể thấy tên của quy tắc, bộ điều kiện và các hành động mà quy tắc sẽ thực hiện.

Để tìm hiểu thêm, hãy xem Tìm [kiếm nhật ký kiểm tra để điều tra các sự cố hỗ trợ phổ biến.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
