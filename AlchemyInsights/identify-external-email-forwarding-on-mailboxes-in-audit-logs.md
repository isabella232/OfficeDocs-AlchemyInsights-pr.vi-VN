---
title: Xác định chuyển tiếp email bên ngoài trên hộp thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508974"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi chuyển tiếp email bên ngoài được cấu hình trên hộp thư

Khi người dùng Microsoft 365 cấu hình chuyển tiếp email bên ngoài vào hộp thư, hoạt động được kiểm toán là một phần của lệnh ghép ngắn **Set-Mailbox** . Bạn có thể xem hoạt động bằng cách sử dụng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật.

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).

2. Đi tới trang **Search**  >  **Tìm kiếm Nhật ký kiểm tra** tìm kiếm.

3. Chọn phạm vi ngày trong ngày **bắt đầu** và **ngày kết thúc** trường. Bạn không cần phải chỉ định tên người dùng. Kiểm tra trường **hoạt động** được đặt để **Hiển thị kết quả cho tất cả các hoạt động**.

4. Nhấp vào **Tìm kiếm**.

Trong kết quả, bấm **lọc kết quả** và loại **bộ hộp thư** trong hộp lọc hoạt động. Chọn bản ghi kiểm tra trong kết quả. Trong hộp thả xuống **chi tiết** , hãy nhấp vào **thêm thông tin**. Bạn phải xem chi tiết của mỗi bản ghi kiểm tra để xác định nếu hoạt động liên quan đến chuyển tiếp email.

- **ObjectID**: bí danh giá trị của hộp thư được thay đổi.

- **Tham số**: giao nhận _dingsmtpaddress_ chỉ email địa chỉ đích.

- **Userid**: người dùng đã định cấu hình chuyển tiếp email trên hộp thư trong trường **ObjectID** .

Để biết thêm thông tin, xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
