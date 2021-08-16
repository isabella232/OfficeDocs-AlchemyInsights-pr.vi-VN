---
title: Sự cố khi mở hoặc tải xuống tệp trong Yammer
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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028278"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Sự cố khi mở hoặc tải xuống tệp trong Yammer

Tính Yammer điển hỗ trợ nhiều tùy chọn để tải tệp lên tin nhắn và nhóm. Tùy thuộc vào cấu hình mạng, tệp mặc định để lưu trữ trong SharePoint.

Bộ chọn tệp trong phiên bản Yammer mới vẫn chưa hỗ trợ tất cả các tùy chọn sẵn dùng trong phiên bản Yammer. Bản cập nhật trong tương lai sẽ thêm các tính năng bổ sung. Để biết thêm thông tin, [hãy xem đính kèm tệp hoặc hình ảnh vào bài đăng Yammer thoại mới](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Không thể mở hoặc tải xuống tệp**  

Tệp có thể tải lên Yammer nhưng cũng có thể liên kết đến tệp trong SharePoint Online. Để khắc phục sự cố, trước tiên bạn phải xác định vị trí của tệp. Nếu tệp đã được tải lên Yammer, tệp sẽ chứa *.yammer.com URL. Đảm bảo rằng các URL và địa chỉ IP được yêu cầu không bị chặn. Để biết thêm thông tin, hãy xem bài đăng blog Sử dụng địa chỉ IP được mã hóa cố [định cho Yammer không được khuyến nghị.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Kiểm tra xem người dùng cũng là người quản trị toàn cầu có thể tải xuống tệp hay không. Nếu tệp đó ở chế độ riêng tư, bạn có thể phải sử dụng Chế độ Nội dung Riêng tư. Để biết thêm thông tin, hãy xem mục [Giám sát nội dung riêng tư trong Yammer.](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)  

**Yammer và tệp mức mạng của bạn trong SharePoint Online**  

[Khách cấp](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) mạng trong Yammer không sử dụng Azure AD B2B và đang nội bộ trong dịch vụ Yammer, vì vậy họ không thể truy nhập vào các tệp Yammer lưu trữ trong SharePoint. Tạo người dùng AAD B2B bên ngoài có thể truy nhập thư viện tài liệu trong SharePoint Online bằng cách sử dụng danh tính đó. Để biết thông tin về hỗ trợ khách Azure AD B2B trong tương lai trong Yammer, xem mục Hỗ trợ doanh nghiệp với doanh nghiệp [(B2B)](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)Hỗ trợ khách trong Yammer Preview - Điều khoản khách hàng và Câu hỏi thường gặp.