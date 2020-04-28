---
title: Thông báo trong yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: ff4c13560b9cbf283e5c6b92a259debdf96cca62
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43911924"
---
# <a name="notifications-in-yammer"></a>Thông báo trong yammer

Để cảnh báo bạn về hoạt động mới trong các cuộc trò chuyện có liên quan, [yammer gửi thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) qua email hoặc — nếu bạn sử dụng yammer trên thiết bị di động — thông qua thông báo đẩy. Theo mặc định, yammer gửi cho bạn thông báo cho nhiều loại hoạt động trong mạng của bạn. Người dùng có thể cập nhật cài đặt email của họ thông qua trang web yammer và đẩy thông báo được cấu hình thông qua ứng dụng di động. 

Yammer đã thêm hỗ trợ cho các [email tương tác trong Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Một số email (bản sao của tin nhắn) sẽ trở thành tương tác trong Outlook trên web. Bản Cập Nhật trong tương lai sẽ mang lại cho các phiên bản khác của Outlook.

**Các loại thông báo trong yammer**

- Email (Cập Nhật từ một nhóm, ai đó mời bạn đến một nhóm, bạn nhận được một tin nhắn trong hộp thư đến của bạn, vv)
- Thông báo đẩy (gửi đến thiết bị di động khi bạn được đề cập, nhận được tin nhắn trong hộp thư đến của bạn, v.v.)
- Popups trên máy tính để bàn (khi bạn đã cài đặt ứng dụng yammer Desktop, nó sẽ hiển thị thông báo cho người dùng được gọi là "Toast" thông báo.)
- Thông báo chuông (bên trong trang web yammer, người dùng sẽ thấy thông báo cho các sự kiện khác nhau. Các thông báo này có thể không luôn có một email hoặc Push Notification liên kết.)

[Thông tin chi tiết về thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) có sẵn.

**Quản lý thông báo**

Người dùng phải quản lý thông báo của riêng họ. Thông tin có sẵn trên [làm thế nào để kích hoạt và vô hiệu hóa yammer email và điện thoại thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Không thể cho quản trị viên vô hiệu hoá tất cả các thông báo hoặc kiểm soát thông báo thay mặt cho người dùng. Quản trị [viên có thể kiểm soát các biểu tượng bao gồm trong email, và cho dù người dùng cần phải xác nhận các tin nhắn](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) được đăng bởi email.

**Thông báo email được gửi đến nhiều người dùng trong tổ chức của bạn**

Đôi khi một thông báo email duy nhất sẽ được gửi bởi yammer và nhận được nhiều người dùng hơn trong tổ chức của bạn hơn mong đợi. Điều này xảy ra khi một danh sách phân phối hoặc các loại địa chỉ email không phải cá nhân được thêm vào yammer. Yammer không biết trong mọi trường hợp, cho dù một địa chỉ email thuộc về một người dùng duy nhất, hoặc là một địa chỉ email mà sẽ gây ra một email được gửi đến nhiều người nhận. Khi sự cố này xảy ra, bạn phải thực hiện hành động để [tạm ngưng (Hủy kích hoạt) người dùng không hợp lệ với địa chỉ email đó](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) trong yammer. 

Để giảm cơ hội của vấn đề này xảy ra, bạn nên:

1. Thực [thi Office 365 nhận dạng](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) yammer.
2. Chặn người gửi bên ngoài gửi email đến tổ chức của bạn hoặc giới hạn người gửi đến danh sách được phê duyệt.

Nếu sự cố này xảy ra:

1. Xác định người nhận email, phải khớp với người dùng trong yammer. Ví dụ, all-in-sales@fabrikam.com là một DL cho tất cả những người bán hàng. DL này sẽ được nhận dạng từ email yammer được người dùng.
2. Sử dụng [tính năng hủy kích hoạt (tạm ngưng) trong quản trị mạng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) để tạm ngưng người dùng có địa chỉ email All-in-Sales@fabrikam.com. Hệ thống treo có thể được hoàn tác, vì vậy an toàn hơn xóa. Xóa người dùng sẽ tự động xảy ra sau 90 ngày.
3. Tùy chọn, xem lại [xuất khẩu người dùng](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) để xác định địa chỉ email không phải người dùng khác sẽ bị treo.
