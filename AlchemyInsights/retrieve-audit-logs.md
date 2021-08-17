---
title: Truy xuất nhật ký kiểm tra
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: 6ca61775d18fb5501911fb3334ef499ff1f06a6b42634367eaf546fc322f822c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889668"
---
# <a name="retrieve-the-audit-logs"></a>Truy xuất nhật ký kiểm tra

Khi bạn mở nhật ký kiểm tra lần đầu, nhật ký kiểm tra sẽ trống. Bạn phải thực hiện tìm kiếm để xem có gì ở đó. Sau đây là cách thực hiện tìm kiếm chung cho tất cả các hoạt động:

1. Thực hiện một trong các bước sau đây:
   - In the Trung tâm tuân thủ Microsoft 365 at <https://compliance.microsoft.com> , go to Solutions  \> **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - Trong cổng thông Bộ bảo vệ Microsoft 365 tại <https://security.microsoft.com> , đi tới Kiểm **tra**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://sip.security.microsoft.com/auditlogsearch> .

2. On the **Audit** page, verify that the **Search** tab is selected and then configure the following settings:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt động**: Xác minh **Hiển thị kết quả cho tất cả các hoạt** động được chọn.
   - **Người dùng:** Chấp nhận giá trị mặc định trống để trả về kết quả cho tất cả người dùng hoặc nhập một hoặc nhiều người dùng.

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Trong kết quả, bấm vào **Lọc Kết quả,** **rồi nhập Set-Mailbox** vào hộp bộ lọc hoạt động.

5. Chọn một bản ghi kiểm tra trong kết quả. Trong khung bật **lên** Chi tiết, **bấm** vào Xem thêm thông tin để xem thêm thông tin như Máy khách, Người dùng đã thực hiện hành động, v.v.
