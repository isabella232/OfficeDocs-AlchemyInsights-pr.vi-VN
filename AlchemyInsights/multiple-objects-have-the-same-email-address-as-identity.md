---
title: Nhiều đối tượng có cùng địa chỉ email với danh tính
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
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724637"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Nhiều đối tượng có cùng địa chỉ email với danh tính

**Nhiều đối tượng**

Một trong những lý do phổ biến của lỗi này không thể định tuyến một yêu cầu Outlook Web Access đúng cách với sự hiện diện của nhiều đối tượng có cùng địa chỉ email với danh tính. Để tìm các đối tượng này, hãy chạy các lệnh sau đây:

· Get-người nhận <email address>

· Get-User <email address>

· Get-User <email address> -softdeleteduser

· Get-liên hệ <email address>

· Tải thư mục được đăng ký hộp thư <email address>

· Get-hộp thư <email address> -includesoftdeletedmailbox

· Get-Mailbox <email address> -inactivemailboxonly

Để giải quyết vấn đề này, hãy loại bỏ nhiều đối tượng với cùng một danh tính email và đảm bảo rằng có một đối tượng duy nhất với danh tính email cụ thể và loại người nhận đó là hộp thư user.

**Cùng một địa chỉ được sử dụng cho các hộp thư kinh doanh và người tiêu dùng**

Nguyên nhân khác là khi cùng một địa chỉ được sử dụng cho các hộp thư kinh doanh và người dùng. Trong trường hợp này, người dùng phải thay đổi biệt danh người tiêu dùng chính của họ cho đến khi Cafe hỗ trợ kịch bản này. Đây là lỗi cố định không biến mất nếu không có can thiệp.

Để biết chi tiết, hãy xem [thay đổi địa chỉ email hoặc số điện thoại cho tài khoản Microsoft của bạn](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).