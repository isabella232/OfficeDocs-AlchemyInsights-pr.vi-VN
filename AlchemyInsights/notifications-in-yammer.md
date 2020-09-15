---
title: Thông báo trong yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: c1fbeea7bf4269e90e52cf5c129e904c99714926
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662815"
---
# <a name="notifications-in-yammer"></a>Thông báo trong yammer

Để cảnh báo bạn về hoạt động mới trong các cuộc hội thoại có liên quan, [yammer sẽ gửi thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) qua email hoặc — nếu bạn sử dụng yammer trên thiết bị di động của mình — qua thông báo đẩy. Theo mặc định, yammer gửi cho bạn thông báo cho nhiều loại hoạt động trong mạng của bạn. Người dùng có thể cập nhật thiết đặt email của họ thông qua website yammer và thông báo đẩy được cấu hình thông qua ứng dụng dành cho thiết bị di động. 

Yammer đã thêm hỗ trợ cho các [email tương tác trong Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Một số email (bản sao của thư) sẽ trở thành tương tác trong Outlook trên web. Bản Cập Nhật trong tương lai sẽ mang đến những phiên bản khác của Outlook.

**Các loại thông báo trong yammer**

- Email (Cập Nhật từ một nhóm, một người nào đó mời bạn đến một nhóm, bạn nhận được một thông báo trong hộp thư đến của bạn, v.v.)
- Thông báo đẩy (được gửi đến thiết bị di động khi bạn được đề cập, nhận được thư trong hộp thư đến của bạn, v.v.)
- Popups trên máy tính (khi bạn đã cài đặt ứng dụng máy tính để bàn yammer, nó sẽ hiển thị thông báo cho người dùng có tên là "Toast" thông báo.)
- Thông báo Bell (bên trong trang web yammer, người dùng sẽ thấy thông báo cho các sự kiện khác nhau. Những thông báo này có thể không phải lúc nào cũng có thông báo gửi email hoặc Push được liên kết.)

[Thông tin chi tiết hơn về thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) sẵn dùng.

**Quản lý thông báo**

Người dùng phải quản lý thông báo của riêng họ. Thông tin sẵn dùng về [cách bật và tắt thông báo về email yammer và di động](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Không thể đối với người quản trị để vô hiệu hóa tất cả thông báo, hoặc điều khiển thông báo, thay mặt cho người dùng. Người quản trị có thể [kiểm soát logo được bao gồm trong email và người dùng có cần xác nhận thư](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) được đăng bằng email hay không.

**Thông báo email được gửi đến nhiều người dùng trong tổ chức của bạn**

Đôi khi một thông báo email duy nhất sẽ được yammer gửi đi và nhận được nhiều người dùng khác trong tổ chức của bạn dự kiến. Điều này sẽ xảy ra khi một danh sách phân phối hoặc các loại địa chỉ email không phải riêng lẻ khác được thêm vào yammer. Yammer không biết trong tất cả các trường hợp, cho dù một địa chỉ email thuộc một người dùng đơn lẻ, hoặc là địa chỉ email sẽ gây ra một email sẽ được gửi đến nhiều người nhận. Khi vấn đề này xảy ra, bạn phải thực hiện hành động để [tạm ngừng (Hủy kích hoạt) người dùng không hợp lệ với địa chỉ email đó](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) trong yammer. 

Để giảm cơ hội xảy ra sự cố này, bạn nên:

1. Áp dụng [danh tính Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) cho yammer.
2. Chặn người gửi bên ngoài gửi email đến tổ chức của bạn hoặc giới hạn người gửi vào một danh sách được phê duyệt.

Nếu sự cố này xảy ra:

1. Xác định người nhận email, vốn sẽ khớp với người dùng trong yammer. Ví dụ, all-in-sales@fabrikam.com là một DL cho tất cả mọi người bán hàng. DL này sẽ được nhận dạng từ email yammer mà người dùng đã nhận.
2. Sử dụng [tính năng hủy kích hoạt (tạm ngừng) trong quản trị mạng](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) để tạm ngừng người dùng có địa chỉ email All-in-Sales@fabrikam.com. Việc tạm ngừng có thể hoàn tác, vì vậy sẽ an toàn hơn so với việc xóa bỏ. Việc xóa người dùng sẽ tự động xảy ra sau 90 ngày.
3. Bạn có thể xem lại việc [xuất người dùng](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) để xác định các địa chỉ email không phải là người dùng khác để bị tạm ngừng.
