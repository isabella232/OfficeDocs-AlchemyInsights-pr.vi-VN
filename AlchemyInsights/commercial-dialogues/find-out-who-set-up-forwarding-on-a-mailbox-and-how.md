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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895201"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Tìm hiểu xem ai thiết lập chuyển tiếp trên hộp thư và cách thức

Nếu chuyển tiếp bên ngoài được đặt trên một hộp thư, hoạt động này sẽ được kiểm tra như một phần của **lệnh ghép ngắn Set-Mailbox.** Sau đây là cách tìm hoạt động trong nhật ký kiểm tra:

1. Thực hiện một trong các thao tác sau:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Nếu bạn thấy thông báo rằng bạn cần bật tính năng kiểm tra, hãy tiếp tục và bật ngay. Nếu tính năng này không được bật, kết quả tìm kiếm sẽ không thể lấy dữ liệu từ ngày trước đó.

2. On the **Audit** page, verify that the **Search** tab is selected and then configure the following settings:
   - Chọn phạm vi ngày/giờ trong hộp **Bắt đầu** **và Kết** thúc.
   - Xác minh hộp Hoạt **động** có chứa kết **quả Hiển thị kết quả cho tất cả các hoạt động.**

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Trong kết quả, bấm vào cột **Hoạt** động để sắp xếp kết quả và tìm mục **nhập Set-Mailbox.**

5. Chọn một hoạt động trong kết quả để mở hộp bật lên chi tiết. Bạn cần xem chi tiết của từng bản ghi kiểm tra để xác định xem hoạt động có liên quan đến chuyển tiếp email không:
   - **ObjectId:** Giá trị biệt danh của hộp thư đã được sửa đổi.
   - **Tham** số : _ForwardingSmtpAddress cho_ biết địa chỉ email đích.
   - **UserId:** Người dùng đã cấu hình chuyển tiếp email trên hộp thư trong **trường ObjectId.**

Để biết thêm thông tin, [xem mục Xác định người thiết lập chuyển tiếp email cho hộp thư.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
