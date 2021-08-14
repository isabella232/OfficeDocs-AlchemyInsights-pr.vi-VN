---
title: Chứng chỉ Đẩy MDM của Apple chưa được thiết lập
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
ms.openlocfilehash: 4f8e3502a7be35b5579ec1436852fe2bff9b1316891c7a9020f6f5f4767b3d88
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931579"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a>Chứng chỉ Đẩy MDM của Apple chưa được thiết lập

Chứng chỉ Đẩy MDM của Apple (còn được gọi là chứng chỉ Dịch vụ Thông báo Đẩy Apple (APNS) không được cấu hình cho đăng ký của bạn. Nếu không cấu hình Chứng chỉ Đẩy MDM của Apple, bạn không thể đăng ký và quản lý các thiết bị iOS và Mac OS. Sau khi bạn thêm chứng chỉ vào Intune, người dùng có thể cài đặt ứng dụng Company Portal để đăng ký thiết bị iOS của họ.

1. Chọn **"Tôi đồng ý."** để cấp cho Microsoft quyền gửi dữ liệu tới Apple.

2. Chọn **Tải xuống CSR của bạn** yêu cầu ký chứng chỉ Intune bắt buộc để tạo chứng chỉ đẩy MDM của Apple. Tệp được sử dụng để yêu cầu chứng chỉ mối quan hệ tin cậy từ Apple Push Certificates Portal.

3. Chọn **Tạo Chứng chỉ đẩy MDM của bạn** để đi đến Apple Push Certificates Portal. Đăng nhập bằng Apple ID công ty của bạn, sau đó chọn **Tạo Chứng chỉ**. Chọn **Chọn Tệp**, duyệt đến tệp yêu cầu ký chứng chỉ, rồi chọn **Tải lên**. Trên trang Xác nhận, chọn **Tải** xuống để tải xuống tệp chứng chỉ (.pem), rồi lưu tệp cục bộ.
 
**Lưu** ý : Chứng chỉ được liên kết với ID Apple được sử dụng để tạo ra nó. Theo kinh nghiệm tốt nhất, hãy dùng Apple ID công ty cho các nhiệm vụ quản lý và đảm bảo hộp thư được giám sát bởi nhiều người hoặc bằng cách sử dụng danh sách phân phối. Không bao giờ sử dụng Apple ID cá nhân. Dùng cùng một Apple ID để gia hạn Chứng chỉ Đẩy Apple mỗi 12 tháng.
 
4. Nhập ID Apple được sử dụng để tạo chứng chỉ đẩy MDM Apple của bạn. Ghi ID này làm lời nhắc khi bạn cần gia hạn chứng chỉ.

5. Đi đến tệp chứng chỉ (.pem), chọn **Mở**, rồi **chọn** Tải lên. Với chứng chỉ đẩy, Intune có thể đăng ký và quản lý các thiết bị Apple.