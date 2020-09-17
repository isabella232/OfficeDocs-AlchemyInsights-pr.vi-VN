---
title: 305 tăng kích cỡ hộp thư lưu trữ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778605"
---
# <a name="increase-the-archive-mailbox-size"></a>Tăng kích cỡ hộp thư lưu trữ


Nếu bạn muốn chúng tôi chạy kiểm tra tự động cho các thiết đặt được đề cập dưới đây, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của người dùng cần kích cỡ hộp thư lưu trữ của họ tăng lên.

Microsoft 365 [giới hạn](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) kích cỡ hộp thư lưu trữ dựa trên giấy phép được gán cho tài khoản người dùng. Khi hộp thư lưu trữ đạt đến 90% kích cỡ được cho phép, người dùng sẽ nhận được thông báo qua email. Khi hộp thư lưu trữ đạt đến giới hạn kích cỡ của nó, người dùng không thể di chuyển các mục khác vào hộp thư lưu trữ. Microsoft 365 sẽ không tăng kích cỡ hộp thư lưu trữ khi đạt đến giới hạn kích cỡ. Thay vào đó, người dùng có thể thực hiện các thao tác sau đây để giải phóng dung lượng trong hộp thư lưu trữ:

- Xuất các mục vào tệp. PST bằng cách dùng Outlook.

- Xóa mục khỏi hộp thư lưu trữ.

Microsoft 365 cung cấp **lưu trữ không giới hạn** đối với các giấy phép Office 365 Enterprise E3 và E5. Người quản trị phải bật tính năng này trước khi hộp thư lưu trữ đạt đến kích cỡ tối đa của nó. Khi việc lưu trữ không giới hạn được bật, có thể mất tối đa 30 ngày trước khi thêm dung lượng miễn phí vào hộp thư lưu trữ. Do đó, chúng tôi khuyên người quản trị xác minh không gian trống trong hộp thư lưu trữ, cho phép người dùng tiếp tục sử dụng hộp thư lưu trữ trong khi nó mở rộng. Để biết thêm thông tin, hãy xem [tổng quan về lưu trữ không giới hạn trong microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) và [bật lưu trữ không giới hạn trong Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Để biết thêm thông tin về việc truy nhập hộp thư lưu trữ từ Outlook, hãy xem các [yêu cầu Outlook để truy nhập các mục trong kho lưu trữ tự động mở rộng](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Để cấu hình chính sách duy trì tự động di chuyển các mục tới hộp thư lưu trữ, hãy xem [thiết lập chính sách lưu trữ và xóa cho hộp thư trong tổ chức Microsoft 365 của bạn](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Lưu ý**: lưu trữ tự động mở rộng không được hỗ trợ đối với hộp thư chính trên Exchange 2010.
