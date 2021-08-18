---
title: Xác định chuyển tiếp email bên ngoài trên hộp thư trong nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 2af731bc9a1e28e2db7c6662041b930e1b05be4c3bf8340784d9ab87101c44af
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899906"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi nào cấu hình chuyển tiếp email bên ngoài trên hộp thư

Khi người Microsoft 365 đặt cấu hình chuyển tiếp email bên ngoài trên hộp thư, hoạt động này được kiểm tra như một phần của lệnh ghép ngắn **Set-Mailbox.** Bạn có thể thấy hoạt động bằng tính năng tìm kiếm nhật ký kiểm tra. Sau đây là cách thực hiện.

1. Thực hiện một trong các bước sau đây:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://sip.security.microsoft.com/auditlogsearch> .

2. On the **Audit** page, verify that the **Search** tab is selected and then configure the following settings:
   - Chọn phạm vi ngày/giờ trong hộp **Bắt đầu** **và Kết** thúc.
   - Xác minh hộp Hoạt **động** có chứa kết **quả Hiển thị kết quả cho tất cả các hoạt động.**

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Trong kết quả, bấm vào **Lọc Kết quả,** **rồi nhập Set-Mailbox** vào hộp bộ lọc hoạt động.

5. Chọn một bản ghi kiểm tra trong kết quả. Trong phần bật **lên Chi** tiết, bấm vào Xem thêm **thông tin.** Bạn cần xem chi tiết của từng bản ghi kiểm tra để xác định xem hoạt động có liên quan đến chuyển tiếp email không.

   - **ObjectId:** Giá trị biệt danh của hộp thư đã được sửa đổi.
   - **Tham** số : _ForwardingSmtpAddress cho_ biết địa chỉ email đích.
   - **UserId:** Người dùng đã cấu hình chuyển tiếp email trên hộp thư trong **trường ObjectId.**

Để biết thêm thông tin, [xem mục Xác định người thiết lập chuyển tiếp email cho hộp thư.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
