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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313521"
---
# <a name="find-events-performed-on-inbox-rules"></a>Tìm các sự kiện được thực hiện trên quy tắc hộp thư đến

Khi các quy tắc hộp thư đến được tạo, thay đổi hoặc xóa, các sự kiện được ghi lại trong nhật ký kiểm tra. Dưới đây là cách xem lại các thay đổi đó:

1. Thực hiện một trong các thao tác sau:
   - Trong thanh công Trung tâm tuân thủ Microsoft 365 , <https://compliance.microsoft.com> đi đến Kiểm tra **Giải** \> **pháp**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - In the Bộ bảo vệ Microsoft 365 portal at <https://security.microsoft.com> , go to **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

    **Lưu** ý: Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể lấy dữ liệu từ ngày trước đó.
1. Chọn trường Hoạt động và tìm hoạt Exchange hộp thư của bạn, rồi chọn New-InboxRule tắc hộp thư đến từ Outlook Web App. Khi bạn thực hiện xong, hãy bấm vào bên ngoài ngăn để thu nhỏ ngăn Hoạt động.
1. Xác định phạm vi ngày, rồi trong trường Người dùng, chọn tên người dùng cho người dùng bạn muốn điều tra. Bạn có thể chọn nhiều người dùng cùng một lúc.
1. Chọn Tìm kiếm. Các hoạt động xuất hiện bên dưới Kết quả.
1. Để xem chi tiết, hãy chọn một hoạt động, rồi chọn Xem thêm Thông tin. Bên dưới phần Tham số, bạn có thể thấy tên của quy tắc, bộ điều kiện và các hành động mà quy tắc sẽ thực hiện.

2. Trên tab Tìm **kiếm** của trang Kiểm **tra,** hãy cấu hình các thiết đặt sau:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt** động : Chọn **Quy tắc Hộp thư đến Mới Tạo quy tắc hộp thư đến từ Outlook Web App**

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Chọn một hoạt động trong kết quả để mở hộp bật lên chi tiết. Bên dưới **phần Tham** số, bạn có thể thấy tên của quy tắc, bộ điều kiện và các hành động mà quy tắc sẽ thực hiện.

Để tìm hiểu thêm, hãy xem Tìm [kiếm nhật ký kiểm tra để điều tra các sự cố hỗ trợ phổ biến.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
