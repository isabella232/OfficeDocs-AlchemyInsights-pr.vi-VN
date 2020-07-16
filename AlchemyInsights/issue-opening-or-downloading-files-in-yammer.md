---
title: Sự cố mở hoặc tải xuống tệp trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148440"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Sự cố mở hoặc tải xuống tệp trong yammer

Cổ điển yammer hỗ trợ nhiều tùy chọn cho tệp tải lên thư và nhóm. Tuỳ thuộc vào cấu hình mạng, tệp mặc định để lưu trữ trong SharePoint.

Bộ chọn tệp trong yammer mới chưa hỗ trợ tất cả các tùy chọn có sẵn trong yammer cổ điển. Bản Cập Nhật trong tương lai sẽ thêm các tính năng bổ sung. Để biết thêm thông tin, xem [đính kèm tệp hoặc hình ảnh vào bài đăng cuộc trò chuyện yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Không thể mở hoặc tải xuống tệp**  

Tệp có thể tải lên yammer nhưng cũng có thể liên kết đến tệp trong SharePoint Online. Để khắc phục sự cố, trước tiên, bạn phải xác định vị trí của tệp. Nếu tập tin đã được tải lên yammer, nó sẽ có một URL *. yammer.com. Đảm bảo rằng URL và địa chỉ IP bắt buộc không bị chặn. Để biết thêm thông tin, hãy xem bài đăng trên blog [bằng cách sử dụng địa chỉ IP cứng mã hoá cho yammer không được khuyến nghị](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Kiểm tra xem người dùng cũng là quản trị viên toàn cầu có thể tải xuống tệp. Nếu tệp là riêng tư, bạn có thể phải sử dụng chế độ nội dung riêng tư. Để biết thêm thông tin, hãy xem sau đó [theo dõi nội dung riêng tư trong yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Khách và tệp ở cấp mạng yammer trong SharePoint Online**  

[Khách hàng cấp mạng trong yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) không sử dụng AZURE AD B2B và nội bộ dịch vụ yammer, do đó, họ không thể truy cập yammer tệp được lưu trữ trong SharePoint. Tạo một bên ngoài AAD B2B người dùng có thể truy cập thư viện tài liệu trong SharePoint trực tuyến bằng cách sử dụng danh tính đó. Để biết thông tin về trong tương lai Azure AD B2B hỗ trợ khách trong yammer, xem [hỗ trợ khách hàng từ doanh nghiệp (B2B) trong yammer Preview-điều khoản khách hàng và câu hỏi thường gặp](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).