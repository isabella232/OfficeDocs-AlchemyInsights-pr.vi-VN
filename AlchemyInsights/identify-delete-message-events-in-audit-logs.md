---
title: Xác định xóa các sự kiện thư trong Nhật ký kiểm tra
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696571"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Nhật ký kiểm tra cho thư email đã xóa

Bắt đầu từ tháng một 2019, Microsoft đang bật tính năng ghi nhật ký kiểm tra hộp thư theo mặc định. Nếu không, để xem lại sự kiện xóa tin nhắn cho một người dùng cụ thể, bạn cần cho phép các hành động xóa để kiểm tra theo cách thủ công. Nếu Nhật ký kiểm tra hộp thư đã được kích hoạt cho tổ chức của bạn hoặc đối với người dùng cụ thể, hãy thực hiện theo các bước dưới đây.

1. Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Microsoft 365](https://protection.office.com/)

2. Bấm **Tìm kiếm và điều tra** và chọn **Tìm kiếm Nhật ký kiểm**tra.

3. Chọn phạm vi ngày trong trường ngày **bắt đầu** và **ngày kết thúc** . Xác định tên người dùng cho người dùng mà bạn muốn điều tra (người dùng đã xóa các mục). Trong trường **hoạt động** , chọn **thư đã xóa khỏi thư mục các mục đã xóa** và thư đã **chuyển vào thư mục các mục đã xóa**.

4. Bấm **Tìm kiếm**.

Trong kết quả, hãy chọn một bản ghi kiểm tra. Trong phần thông tin chi tiết, hãy bấm **xem thêm thông tin**. Thông tin bổ sung về mục đã xóa (ví dụ, dòng chủ đề và vị trí của mục khi thư đã bị xóa) được hiển thị trong trường **Affecteditems** . Thuộc tính **Clientinfostring** sẽ hiển thị nếu việc xóa đã xảy ra trong Outlook, Outlook trên web (trước đây gọi là Outlook Web App) hoặc bất kỳ thiết bị nào khác.

Để biết thêm thông tin, hãy xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Lưu ý**: bạn không thể truy xuất các mục đã xóa bằng tính năng Nhật ký kiểm tra. Để truy xuất thư đã xóa trong Outlook trên web, hãy xem [khôi phục các mục đã xóa trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
