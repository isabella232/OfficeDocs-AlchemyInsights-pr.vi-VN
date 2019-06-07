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
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752044"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi chuyển tiếp email bên ngoài được cấu hình trên hộp thư

Khi người dùng cấu hình chuyển tiếp thư điện tử bên ngoài một hộp thư, các hoạt động kiểm toán là một phần của lệnh ghép ngắn **Set-Mailbox** . Bạn có thể xem các hoạt động bằng cách sử dụng kiểm toán đăng nhập tìm kiếm trong an ninh & Trung tâm phù hợp.

1. Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)

2. Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.

3. Chọn phạm vi ngày trong các **ngày bắt đầu** và **ngày kết thúc** . Bạn không cần phải chỉ định một tên người dùng. Xác minh các lĩnh vực **hoạt động** được đặt để **Hiển thị kết quả cho tất cả các hoạt động**.

4. Nhấp vào **Tìm kiếm**.

Trong kết quả, hãy nhấp vào **Bộ lọc kết quả** và loại **Set-Mailbox** trong hộp lọc hoạt động. Hãy chọn một hồ sơ kiểm toán trong các kết quả. Trong flyout **chi tiết** , bấm vào **thêm thông tin**. Bạn cần phải xem xét các chi tiết của mỗi hồ sơ kiểm toán để xác định nếu các hoạt động có liên quan đến email chuyển tiếp.

- **ObjectId**: giá trị bí danh của hộp thư đã được thay đổi.

- **Thông số**: _ForwardingSmtpAddress_ địa chỉ email mục tiêu cho biết.

- **User**: người dùng đã đặt cấu hình chuyển tiếp email trong hộp thư trong lĩnh vực **ObjectId** .

Để biết thêm chi tiết, hãy xem [Determining người thiết lập email chuyển tiếp cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
