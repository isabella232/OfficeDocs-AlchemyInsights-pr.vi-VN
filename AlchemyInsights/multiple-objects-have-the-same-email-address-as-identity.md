---
title: Nhiều đối tượng có cùng địa chỉ email như danh tính
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
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439705"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Nhiều đối tượng có cùng địa chỉ email như danh tính

**Nhiều đối tượng**

Một trong những lý do phổ biến của lỗi này không thể định tuyến một yêu cầu Outlook Web Access đúng trong sự hiện diện của nhiều đối tượng có cùng địa chỉ email như danh tính. Để tìm các đối tượng này, hãy chạy lệnh sau:

· Nhận-người nhận<email address>

· Get-người dùng<email address>

· Nhận-người dùng <email address> -softdeleteduser

· Get-liên hệ<email address>

· Nhận hộp thư <email address> -publicfolder

· Nhận hộp thư <email address> -includesoftdeletedmailbox

· Nhận được-Mailbox <email address> -inactivemailboxonly

Để khắc phục sự cố, loại bỏ nhiều đối tượng với nhận dạng email cùng và đảm bảo rằng có một đối tượng duy nhất với danh tính email cụ thể và loại người nhận là UserMailbox.

**Cùng một địa chỉ được sử dụng cho doanh nghiệp và người tiêu dùng hộp thư**

Nguyên nhân khác là khi cùng một địa chỉ được sử dụng cho doanh nghiệp và người tiêu dùng hộp thư. Trong trường hợp này, người dùng phải thay đổi bí danh tiêu dùng chính của họ cho đến khi Cafe hỗ trợ kịch bản này. Đây là một lỗi vĩnh viễn mà không đi xa mà không can thiệp.

Để biết chi tiết, hãy xem [thay đổi địa chỉ email hoặc số điện thoại cho tài khoản Microsoft của bạn](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).