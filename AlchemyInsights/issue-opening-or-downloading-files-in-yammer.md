---
title: Sự cố khi mở hoặc tải xuống các tệp trong yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695671"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Sự cố khi mở hoặc tải xuống các tệp trong yammer

Yammer cổ điển hỗ trợ nhiều tùy chọn để tải lên tệp tin nhắn và nhóm. Tùy thuộc vào cấu hình mạng, các tệp mặc định là lưu trữ trong SharePoint.

Bộ chọn tệp trong mới yammer vẫn chưa hỗ trợ tất cả các tùy chọn sẵn dùng trong yammer cổ điển. Bản Cập Nhật trong tương lai sẽ thêm các tính năng bổ sung. Để biết thêm thông tin, hãy xem [đính kèm tệp hoặc hình ảnh vào bài đăng hội thoại yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Không thể mở hoặc tải xuống tệp**  

Một tệp có thể tải lên yammer mà còn được liên kết đến một tệp trong SharePoint Online. Để khắc phục sự cố, trước tiên, bạn phải xác định vị trí của tệp. Nếu tệp đã được tải lên yammer, nó sẽ có URL *. yammer.com. Đảm bảo rằng các URL và địa chỉ IP được yêu cầu không bị chặn. Để biết thêm thông tin, hãy xem bài đăng blog [bằng địa chỉ IP được mã hóa cứng cho yammer không được đề](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)xuất.

Kiểm tra xem người dùng cũng là người quản trị toàn cầu có thể tải xuống tệp hay không. Nếu tệp là riêng tư, bạn có thể phải sử dụng chế độ nội dung riêng tư. Để biết thêm thông tin, hãy xem sau đó [giám sát nội dung riêng tư trong yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Các khách hàng và các tệp cấp độ mạng yammer trong SharePoint Online**  

Các [khách hàng ở mức mạng trong yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) không sử dụng AZURE AD B2B và nằm bên trong dịch vụ yammer, vì vậy họ không thể truy nhập các tệp yammer được lưu trữ trong SharePoint. Tạo một người dùng B2B bên ngoài người dùng có thể truy nhập vào thư viện tài liệu trong SharePoint Online bằng cách sử dụng danh tính đó. Để biết thông tin về việc tương lai Azure AD B2B hỗ trợ khách trong yammer, hãy xem [hỗ trợ khách mời Business-to-Business (B2B) trong bản xem trước yammer-các điều khoản và câu hỏi thường gặp của khách hàng](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).