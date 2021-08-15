---
title: 'Lỗi: Các quy tắc trên máy tính này không khớp'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981135"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>Lỗi: Các quy tắc trên máy tính này không khớp

Để xem trạng thái cập nhật của sự cố đã biết này, hãy xem các quy tắc trên máy tính [này không khớp](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) với các quy tắc trên Microsoft Exchange

Nhóm Outlook đã triển khai bản sửa lỗi trong Bản dựng 12928.10000. Bản sửa lỗi đã có mặt tại Người dùng nội bộ Nhanh và sẽ đi đến Kênh hàng tháng vào cuối Tháng Sáu 2020. Sau khi đã khắc phục, bạn có thể nhận được lời nhắc "Bạn muốn giữ quy tắc nào" lần cuối. Chọn Máy chủ khi được nhắc, rồi quay lại Outlook bật lại bất kỳ quy tắc nào đã bị tắt.

Cho đến khi có bản sửa lỗi, vui lòng sử dụng giải pháp thay thế sau:

**Giải pháp thay thế**: Trong các báo cáo gần đây, sự cố đã xảy ra đối với những báo cáo chỉ tạo quy tắc máy khách trong máy Outlook tính. Nếu bạn tiếp tục gặp sự cố, hãy xem xét việc xóa các quy tắc, rồi tạo và chỉnh sửa các quy tắc chỉ trong OWA (Outlook Web App) cho đến khi sự cố được giải quyết.

Nếu bạn không thể xóa quy tắc theo cách thủ công, bạn có thể chạy lệnh Outlook khi bắt đầu Outlook quy tắc bằng cách chạy Outlook.exe /cleanrules. Điều này sẽ xóa cả quy tắc máy khách và máy chủ. Nó sẽ xóa bỏ tất cả quy tắc cho tất cả các tài khoản trong Hồ Outlook của bạn. Lệnh này được ghi lại thêm trong bài viết Khóa chuyển Dòng lệnh.

