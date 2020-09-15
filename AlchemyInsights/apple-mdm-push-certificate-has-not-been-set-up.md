---
title: Chứng chỉ đẩy táo MDM đã không được thiết lập
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716879"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Chứng chỉ đẩy táo MDM đã không được thiết lập

Chứng chỉ đẩy của Apple MDM (còn được gọi là chứng chỉ dịch vụ thông báo đẩy táo) chưa được cấu hình cho đăng ký của bạn. Nếu không có giấy chứng nhận đẩy táo MDM được cấu hình, bạn sẽ không thể đăng ký và quản lý các thiết bị chạy iOS và Mac OS. Sau khi bạn thêm chứng chỉ vào InTune, người dùng có thể cài đặt ứng dụng cổng thông tin công ty để đăng ký thiết bị iOS của họ.

1. Chọn **"Tôi đồng ý".** để cấp quyền cho Microsoft để gửi dữ liệu sang Apple.

2. Chọn **tải xuống** yêu cầu đăng nhập chứng chỉ không điều chỉnh của bạn được yêu cầu để tạo chứng chỉ đẩy MDM của Apple. Tệp được dùng để yêu cầu chứng chỉ mối quan hệ tin cậy từ cổng thông tin chứng chỉ đẩy táo.

3. Chọn **tạo chứng chỉ đẩy MDM của bạn** để đi đến cổng thông tin chứng chỉ Push của Apple. Đăng nhập bằng ID Apple của công ty bạn, rồi chọn **tạo chứng chỉ**. Chọn **chọn tệp**, duyệt đến tệp yêu cầu ký chứng chỉ, rồi chọn **tải lên**. Trên trang xác nhận, chọn **tải xuống** để tải xuống tệp chứng chỉ (. pem) và lưu tệp cục bộ.
 
**Lưu ý**: chứng chỉ được liên kết với Apple ID được sử dụng để tạo ra. Với tư cách là tốt nhất, hãy sử dụng một công ty Apple ID cho các tác vụ quản lý và đảm bảo rằng hộp thư được theo dõi bởi nhiều người hoặc bằng cách sử dụng danh sách phân phối. Không bao giờ sử dụng ID cá nhân của Apple. Sử dụng cùng một ID Apple để gia hạn chứng chỉ đẩy táo mỗi 12 tháng.
 
4. Nhập Apple ID được dùng để tạo chứng chỉ đẩy MDM táo của bạn. Ghi lại ID này làm lời nhắc khi bạn cần gia hạn chứng chỉ.

5. Đi đến tệp chứng chỉ (. pem), chọn **mở**, rồi chọn **tải lên**. Với chứng chỉ đẩy, InTune có thể đăng ký và quản lý các thiết bị của Apple.