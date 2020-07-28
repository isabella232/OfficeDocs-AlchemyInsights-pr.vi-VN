---
title: Apple MDM Push Certificate chưa được thiết lập
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440005"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Apple MDM Push Certificate chưa được thiết lập

Apple MDM Push Certificate (còn được gọi là chứng chỉ Apple Push Notification Service (APNS)) chưa được cấu hình cho đăng ký của bạn. Nếu không có một Apple MDM Push Certificate cấu hình, bạn không thể đăng ký và quản lý các thiết bị iOS và Mac OS. Sau khi bạn thêm chứng chỉ dành cho InTune, người dùng có thể cài đặt ứng dụng cổng thông tin công ty để đăng ký thiết bị iOS của họ.

1. Chọn **"Tôi đồng ý".** để cho phép Microsoft gửi dữ liệu đến Apple.

2. Chọn **tải xuống CSR của bạn** yêu cầu đăng ký chứng chỉ cần thiết để tạo một Apple MDM đẩy chứng chỉ. Tệp được sử dụng để yêu cầu chứng chỉ mối quan hệ tin cậy từ cổng của Apple Push Certificate.

3. Chọn **tạo chứng chỉ đẩy MDM của bạn** để đi đến cổng thông tin chứng chỉ Push của Apple. Đăng nhập bằng ID Apple của công ty, sau đó chọn **tạo chứng chỉ**. Chọn **chọn tệp**, duyệt đến tệp yêu cầu ký chứng chỉ và sau đó chọn **tải lên**. Trên trang xác nhận, chọn **tải xuống** để tải xuống tệp chứng chỉ (. pem) và lưu tệp cục bộ.
 
**Lưu ý**: chứng chỉ được liên kết với Apple ID được sử dụng để tạo ra nó. Để thực hành tốt nhất, hãy sử dụng Apple ID của công ty cho các tác vụ quản lý và đảm bảo rằng hộp thư được giám sát bởi nhiều người hoặc bằng cách sử dụng danh sách phân phối. Không bao giờ sử dụng ID Apple cá nhân. Sử dụng cùng một Apple ID để gia hạn giấy chứng nhận của Apple Push Certificate mỗi 12 tháng.
 
4. Nhập Apple ID được sử dụng để tạo giấy chứng nhận đẩy Apple MDM của bạn. Ghi lại ID này như một lời nhắc nhở khi bạn cần gia hạn chứng chỉ.

5. Đi tới tệp chứng chỉ (. pem), chọn **mở**, sau đó chọn **tải lên**. Với giấy chứng nhận đẩy, InTune có thể đăng ký và quản lý các thiết bị của Apple.