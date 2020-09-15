---
title: Xác định chuyển tiếp email bên ngoài trên các hộp thư trong Nhật ký kiểm tra
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696319"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi chuyển tiếp email bên ngoài được đặt cấu hình trên hộp thư

Khi người dùng Microsoft 365 đặt cấu hình chuyển tiếp email bên ngoài trên một hộp thư, hoạt động được kiểm toán như là một phần của lệnh ghép ngắn **Set-Mailbox** . Bạn có thể thấy hoạt động bằng cách sử dụng tính năng tìm kiếm Nhật ký kiểm tra trong Trung tâm tuân thủ & bảo mật.

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/).

2. Đi đến trang **Search**  >  **Tìm kiếm Nhật ký kiểm** tra tìm kiếm.

3. Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** . Bạn không cần phải xác định tên người dùng. Xác minh trường **hoạt động** được thiết lập để **Hiển thị kết quả cho tất cả các hoạt động**.

4. Bấm **Tìm kiếm**.

Trong kết quả, bấm vào **lọc kết quả** và gõ **Set-Mailbox** trong hộp bộ lọc hoạt động. Chọn một bản ghi kiểm tra trong kết quả. Trong phần **thông tin chi tiết** , hãy bấm **xem thêm thông tin**. Bạn phải xem chi tiết của từng bản ghi kiểm tra để xác định xem hoạt động có liên quan đến chuyển tiếp email hay không.

- **ObjectID**: giá trị biệt danh của hộp thư đã được sửa đổi.

- **Tham số**: chuyển tiếp biểu thị _địa chỉ email_ đích.

- **Userid**: người dùng đã cấu hình chuyển tiếp email trên hộp thư trong trường **ObjectID** .

Để biết thêm thông tin, hãy xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
