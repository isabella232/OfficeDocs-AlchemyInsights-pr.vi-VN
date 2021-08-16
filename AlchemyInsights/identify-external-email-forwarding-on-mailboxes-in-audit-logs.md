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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028780"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Xác định khi nào cấu hình chuyển tiếp email bên ngoài trên hộp thư

Khi người dùng Microsoft 365 cấu hình chuyển tiếp email bên ngoài trên một hộp thư, hoạt động này được kiểm tra như một phần của lệnh ghép ngắn **Set-Mailbox.** Bạn có thể thấy hoạt động sử dụng tính năng tìm kiếm nhật ký kiểm tra trong Trung tâm & tuân thủ Bảo mật.

1. Đăng nhập vào Trung [tâm Microsoft 365 Tuân thủ .](https://protection.office.com/)

2. Đi đến trang Tìm **kiếm nhật** ký  >  **kiểm tra.**

3. Chọn phạm vi ngày trong các **trường Ngày bắt đầu** và Ngày **kết** thúc. Bạn không cần chỉ định tên người dùng. Xác minh trường **Hoạt động** được đặt thành Hiển thị kết quả cho tất cả các **hoạt động.**

4. Bấm Tìm **kiếm.**

Trong kết quả, bấm vào **Lọc Kết quả,** **rồi nhập Set-Mailbox** vào hộp bộ lọc hoạt động. Chọn một bản ghi kiểm tra trong kết quả. Trong phần bật **lên Chi** tiết, bấm vào Xem thêm **thông tin.** Bạn phải xem chi tiết của từng bản ghi kiểm tra để xác định xem hoạt động có liên quan đến chuyển tiếp email không.

- **ObjectId:** Giá trị biệt danh của hộp thư đã được sửa đổi.

- **Tham** số : _ForwardingSmtpAddress cho_ biết địa chỉ email đích.

- **UserId:** Người dùng đã cấu hình chuyển tiếp email trên hộp thư trong **trường ObjectId.**

Để biết thêm thông tin, [xem mục Xác định người thiết lập chuyển tiếp email cho hộp thư.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
