---
title: Xác định xóa sự kiện thư trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716518"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Nhật ký kiểm tra cho thư email đã xóa

Bắt đầu từ tháng 2019, Microsoft đang bật kiểm tra hộp thư đăng nhập theo mặc định. Nếu không, để xem lại xóa sự kiện tin nhắn cho một người dùng cụ thể, bạn cần phải bật thủ công các hành động xóa để kiểm tra. Nếu hộp kiểm tra ghi nhật ký đã được kích hoạt cho tổ chức của bạn hoặc cho người dùng cụ thể, hãy làm theo các bước dưới đây.

1. Đăng nhập vào [Microsoft 365 bảo mật & tuân thủ trung tâm](https://protection.office.com/)

2. Nhấp vào **Tìm kiếm và điều tra** và chọn **Tìm kiếm Nhật ký kiểm tra**.

3. Chọn phạm vi ngày trong ngày **bắt đầu** và **ngày kết thúc** trường. Chỉ định tên người dùng mà bạn muốn điều tra (người dùng đã xoá các mục). Trong trường **hoạt động** , chọn thư **đã xoá từ thư mục mục đã xoá** và **di chuyển thư vào thư mục mục đã xóa**.

4. Nhấp vào **Tìm kiếm**.

Trong kết quả, chọn bản ghi kiểm tra. Trong thông tin chi tiết flyout, hãy nhấp vào **Thêm**. Thông tin bổ sung về mục đã xoá (ví dụ: dòng chủ đề và vị trí của mục khi nó đã bị xoá) được hiển thị trong trường **Affecteditems** . Thuộc tính **Clientinfostring** sẽ hiển thị nếu xóa xảy ra trong Outlook, Outlook trên web (trước đây được gọi là Outlook Web App) hoặc bất kỳ thiết bị nào khác.

Để biết thêm thông tin, xem [xác định người thiết lập chuyển tiếp email cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Lưu ý**: bạn không thể truy xuất các mục đã xóa bằng tính năng Nhật ký kiểm tra. Để lấy các thư đã xóa trong Outlook trên web, hãy xem [khôi phục các mục đã xóa trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
