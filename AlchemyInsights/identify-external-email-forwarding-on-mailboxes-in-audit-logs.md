---
title: Xác định bên ngoài email chuyển tiếp vào hộp thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539123"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi chuyển tiếp email bên ngoài được cấu hình trên hộp thư

Khi một người dùng Office 365 cấu hình chuyển tiếp thư điện tử bên ngoài một hộp thư, các hoạt động kiểm toán là một phần của lệnh ghép ngắn **Set-Mailbox** . Bạn có thể xem các hoạt động bằng cách sử dụng kiểm toán đăng nhập tìm kiếm trong an ninh & Trung tâm phù hợp.

1. Đăng nhập [Office 365 an ninh & tuân thủ trung tâm](https://protection.office.com/).

2. Đi **Tìm** > trang**kiểm toán đăng nhập tìm kiếm** .

3. Chọn phạm vi ngày trong các **ngày bắt đầu** và **ngày kết thúc** . Bạn không cần phải chỉ định một tên người dùng. Xác minh các lĩnh vực **hoạt động** được đặt để **Hiển thị kết quả cho tất cả các hoạt động**.

4. Nhấp vào **Tìm kiếm**.

Trong kết quả, hãy nhấp vào **Bộ lọc kết quả** và loại **Set-Mailbox** trong hộp lọc hoạt động. Hãy chọn một hồ sơ kiểm toán trong các kết quả. Trong flyout **chi tiết** , bấm vào **thêm thông tin**. Bạn cần phải xem xét các chi tiết của mỗi hồ sơ kiểm toán để xác định nếu các hoạt động có liên quan đến email chuyển tiếp.

- **ObjectId**: giá trị bí danh của hộp thư đã được thay đổi.

- **Thông số**: _ForwardingSmtpAddress_ địa chỉ email mục tiêu cho biết.

- **User**: người dùng đã đặt cấu hình chuyển tiếp email trong hộp thư trong lĩnh vực **ObjectId** .

Để biết thêm chi tiết, hãy xem [Determining người thiết lập email chuyển tiếp cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
