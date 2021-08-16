---
title: Thông báo trong Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097220"
---
# <a name="notifications-in-yammer"></a>Thông báo trong Yammer

Để cảnh báo cho bạn về hoạt động mới trong các cuộc hội thoại có liên quan, [Yammer](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) sẽ gửi thông báo qua email hoặc—nếu bạn sử dụng Yammer trên thiết bị di động—thông qua thông báo đẩy. Theo mặc định, Yammer sẽ gửi cho bạn thông báo về nhiều loại hoạt động trong mạng của bạn. Người dùng có thể cập nhật thiết đặt email của họ thông qua website Yammer và thông báo đẩy được cấu hình thông qua ứng dụng dành cho thiết bị di động. 

Yammer đã bổ sung hỗ trợ [cho email tương tác trong Outlook.](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420) Một số email (bản sao của thư) sẽ có tính tương tác trong Outlook trên web. Bản cập nhật trong tương lai sẽ đưa bản cập nhật này đến các phiên bản khác của Outlook.

**Các loại thông báo trong Yammer**

- Email (Các cập nhật từ một nhóm, ai đó mời bạn vào một nhóm, bạn sẽ nhận được thư trong hộp thư đến của bạn, v.v.)
- Thông báo đẩy (Được gửi đến thiết bị di động khi bạn được đề cập, nhận tin nhắn trong hộp thư đến của bạn, v.v.)
- Cửa sổ bật lên trên máy tính (Khi bạn cài đặt ứng dụng Yammer trên máy tính, ứng dụng sẽ hiển thị thông báo cho người dùng gọi là thông báo "thông báo".)
- Thông báo hình chuông (Bên trong Yammer trang web, người dùng sẽ thấy thông báo về các sự kiện khác nhau. Không phải lúc nào những thông báo này cũng có thể có email liên kết hoặc thông báo đẩy.)

Thông tin [chi tiết hơn về thông báo](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) có sẵn.

**Quản lý thông báo**

Người dùng phải quản lý thông báo của riêng họ. Thông tin có sẵn về [cách bật và tắt thông báo Yammer email và di động.](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) 

Người quản trị không thể tắt tất cả thông báo hoặc điều khiển thông báo thay mặt người dùng. Người quản trị có [thể điều khiển logo được tích hợp trong email và liệu người dùng có cần xác nhận những thông điệp được](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) đăng qua email hay không.

**Thông báo qua email được gửi cho nhiều người dùng trong tổ chức của bạn**

Đôi khi, nhiều người dùng trong tổ chức của bạn sẽ nhận được Yammer một thông báo email đơn lẻ và được nhiều người dùng trong tổ chức của bạn gửi và nhận. Điều này xảy ra khi danh sách phân phối hoặc loại địa chỉ email không phải cá nhân khác, được thêm vào danh Yammer. Yammer trong mọi trường hợp, liệu địa chỉ email có thuộc về người dùng đơn lẻ hay là địa chỉ email sẽ khiến cho một email gửi đến nhiều người nhận. Khi sự cố này xảy ra, bạn phải hành động để tạm ngừng (hủy kích [hoạt)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) người dùng không hợp lệ với địa chỉ email đó trong Yammer. 

Để giảm khả năng xảy ra sự cố này, bạn nên:

1. [Thực thi Office 365 tính người](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) dùng cho Yammer.
2. Chặn người gửi bên ngoài gửi email đến tổ chức của bạn hoặc giới hạn người gửi trong danh sách đã phê duyệt.

Nếu sự cố này xảy ra:

1. Xác định người nhận email khớp với người dùng trong Yammer. Ví dụ: all-in-sales@fabrikam.com là DL cho tất cả nhân viên bán hàng. DL này sẽ được nhận dạng từ email Yammer người dùng nhận được.
2. Sử dụng [tính năng hủy kích hoạt (tạm ngừng)](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) trong Quản trị Mạng để tạm ngừng người dùng có địa chỉ all-in-sales@fabrikam.com email. Tạm ngừng có thể được hoàn tác, vì vậy sẽ an toàn hơn xóa. Việc xóa người dùng sẽ diễn ra tự động sau 90 ngày.
3. Hoặc, xem lại xuất người [dùng để](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) xác định các địa chỉ email không phải người dùng khác sẽ bị tạm ngừng.
