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
ms.openlocfilehash: ac2e5eafbb92b234697c22f73cd565af9d7c3508
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329516"
---
# <a name="retrieve-the-audit-logs"></a>Truy xuất nhật ký kiểm tra

Khi bạn mở nhật ký kiểm tra lần đầu, nhật ký kiểm tra sẽ trống. Bạn phải thực hiện tìm kiếm để xem có gì ở đó. Sau đây là cách thực hiện tìm kiếm chung cho tất cả các hoạt động:

1. Thực hiện một trong các bước sau đây:
   - Trong thanh công Trung tâm tuân thủ Microsoft 365 , <https://compliance.microsoft.com> đi đến Kiểm tra **Giải** \> **pháp**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - In the Bộ bảo vệ Microsoft 365 portal at <https://security.microsoft.com> , go to **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://sip.security.microsoft.com/auditlogsearch> .

2. On the **Audit** page, verify that the **Search** tab is selected and then configure the following settings:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt động**: Xác minh **Hiển thị kết quả cho tất cả các hoạt** động được chọn.
   - **Người dùng:** Chấp nhận giá trị mặc định trống để trả về kết quả cho tất cả người dùng hoặc nhập một hoặc nhiều người dùng.

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Trong kết quả, bấm vào **Lọc Kết quả,** **rồi nhập Set-Mailbox** vào hộp bộ lọc hoạt động.

5. Chọn một bản ghi kiểm tra trong kết quả. Trong khung bật **lên** Chi tiết, **bấm** vào Xem thêm thông tin để xem thêm thông tin như Máy khách, Người dùng đã thực hiện hành động, v.v.
