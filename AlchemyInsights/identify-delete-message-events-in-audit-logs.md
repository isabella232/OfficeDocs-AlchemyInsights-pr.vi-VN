---
title: Xác định sự kiện thông báo xóa trong Nhật ký kiểm tra
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539231"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Nhật ký kiểm tra cho các thư email đã xoá

Bắt đầu từ năm 2019, Microsoft là chuyển vào hộp thư kiểm tra đăng nhập theo mặc định. Nếu không, để xem xét xóa các sự kiện tin nhắn cho một người dùng cụ thể, bạn cần bật bằng tay các hành động delete đối với kiểm toán. Nếu hộp kiểm toán đăng nhập đã được kích hoạt cho tổ chức của bạn hoặc cho người dùng cụ thể, hãy làm theo các bước dưới đây.

1. Đăng nhập vào [Trung tâm Compliance Office 365 bảo mật &](https://protection.office.com/)

2. Nhấp vào **Tìm kiếm và điều tra** và chọn **Kiểm toán đăng nhập tìm kiếm**.

3. Chọn phạm vi ngày trong các **ngày bắt đầu** và **ngày kết thúc** . Chỉ định tên đăng nhập cho người dùng mà bạn muốn để điều tra (người dùng xóa các mục). Trong lĩnh vực **hoạt động** , lựa chọn **đã bị xoá thư khỏi thư mục mục đã xoá** và **chuyển thư đến thư mục mục đã xoá**.

4. Nhấp vào **Tìm kiếm**.

Trong các kết quả, hãy chọn một hồ sơ kiểm toán. Trong flyout chi tiết, bấm vào **Thêm thông tin**. Các thông tin bổ sung về mục đã xoá (ví dụ, dòng tiêu đề và vị trí các mục khi đã bị xóa) sẽ được hiển thị trong lĩnh vực **AffectedItems** . Bất động sản **ClientInfoString** sẽ hiển thị nếu việc xoá bỏ xảy ra trong Outlook, Outlook trên web (trước đây gọi là Outlook Web App), hoặc bất kỳ thiết bị nào khác.

Để biết thêm chi tiết, hãy xem [Determining người thiết lập email chuyển tiếp cho một hộp thư](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Lưu ý**: bạn không thể truy xuất khoản mục đã xóa bằng cách sử dụng tính năng đăng nhập kiểm toán. Để truy lục thư đã xoá trong Outlook trên web, hãy xem [khôi phục đã xoá các mục trong Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
