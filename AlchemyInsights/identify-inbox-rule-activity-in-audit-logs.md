---
title: Xác định hoạt động quy tắc hộp thư đến trong nhật ký kiểm tra
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331145"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Xác định hoạt động quy tắc hộp thư đến trong nhật ký kiểm tra

Bạn có thể sử dụng tìm kiếm nhật ký kiểm tra trong Trung tâm tuân thủ Microsoft 365 để xem các sự kiện về quy tắc hộp thư đến (tạo, sửa đổi và xóa quy tắc hộp thư đến).

1. Thực hiện một trong các bước sau đây:
   - Trong thanh công Trung tâm tuân thủ Microsoft 365 , <https://compliance.microsoft.com> đi đến Kiểm tra **Giải** \> **pháp**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://compliance.microsoft.com/auditlogsearch> .
   - In the Bộ bảo vệ Microsoft 365 portal at <https://security.microsoft.com> , go to **Audit**. Hoặc để đi trực tiếp đến trang **Kiểm tra,** sử dụng <https://security.microsoft.com/auditlogsearch> .

2. Trên tab Tìm **kiếm** của trang Kiểm **tra,** hãy cấu hình các thiết đặt sau:
   - **Phạm vi ngày và giờ**: Chọn phạm vi ngày/giờ trong hộp Bắt **đầu** **và Kết** thúc.
   - **Hoạt** động : Chọn một hoặc nhiều giá trị sau đây:
     - **Quy tắc Hộp thư đến Mới Tạo quy tắc hộp thư đến từ Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Cập nhật quy tắc hộp thư đến từ máy Outlook khách**

3. Khi bạn hoàn tất, hãy bấm Tìm **kiếm.** Các hoạt động sẽ xuất hiện trên trang **Tìm kiếm kiểm tra** mới.

4. Chọn một hoạt động trong kết quả để mở hộp bật lên chi tiết. Thông tin về thiết đặt quy tắc hộp thư đến được hiển thị trong **trường Tham** số.

Để biết thêm thông tin, xem [mục Xác định người dùng đã tạo quy tắc hộp thư đến](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
