---
title: Xác định các sự kiện thư bị xóa trong nhật ký kiểm tra
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630091"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Nhật ký kiểm tra thư email đã xóa

Bắt đầu từ Tháng Một 2019, Microsoft sẽ bật tính năng ghi nhật ký kiểm tra hộp thư theo mặc định. Nếu không, để xem lại các sự kiện xóa thư cho một người dùng cụ thể, bạn cần phải bật thủ công các hành động xóa để kiểm tra. Nếu tính năng ghi nhật ký kiểm tra hộp thư đã được bật cho tổ chức của bạn hoặc cho người dùng cụ thể, hãy làm theo các bước dưới đây.

1. Đăng nhập vào Trung [tâm Microsoft 365 Tuân thủ](https://protection.office.com/)

2. Bấm Tìm **kiếm và Điều tra và** chọn Tìm kiếm Nhật ký Kiểm **tra.**

3. Chọn phạm vi ngày trong các **trường Ngày bắt đầu** và Ngày **kết** thúc. Chỉ định tên người dùng cho người dùng mà bạn muốn điều tra (người dùng đã xóa các mục). Trong trường Hoạt **động,** chọn Thư **đã xóa từ thư mục Các mục Đã xóa và** Thư đã di chuyển vào thư mục Các mục Đã **xóa**.

4. Bấm Tìm **kiếm.**

Trong kết quả, hãy chọn một bản ghi kiểm tra. Trong phần bật ra chi tiết, bấm vào Xem **thêm Thông tin**. Thông tin bổ sung về mục đã xóa (ví dụ: dòng chủ đề và vị trí của mục khi mục bị xóa) được hiển thị trong trường Mục **bị Ảnh** hưởng. Thuộc **tính ClientInfoString** sẽ hiển thị nếu việc xóa xảy ra trong Outlook, Outlook trên web (trước đây được gọi là Outlook Web App) hoặc bất kỳ thiết bị nào khác.

Để biết thêm thông tin, [xem mục Xác định người thiết lập chuyển tiếp email cho hộp thư.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Lưu ý:** Bạn không thể truy xuất các mục đã xóa bằng tính năng nhật ký kiểm tra. Để truy xuất thư đã xóa trong Outlook trên web, hãy xem [Khôi phục các mục đã xóa Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
