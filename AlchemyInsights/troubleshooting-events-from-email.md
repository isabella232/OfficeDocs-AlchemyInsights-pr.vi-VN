---
title: Khắc phục sự kiện từ email
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
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658756"
---
# <a name="troubleshooting-events-from-email"></a>Khắc phục sự kiện từ email

1. Xác nhận tính năng được kích hoạt cho hộp thư: **Get-Eventsfroconfiguration-danh <mailbox> tính**

2. Sau đó, hãy xem mục các sự kiện ' từ xuất Nhật ký của email **-MailboxDiagnosticLogs <mailbox> -khung hồ sơ thành phần**

3. Trong Nhật ký ' các sự kiện từ email, hãy tìm InternetMessageId khớp với mục đó trong hộp thư.  

4. Trustđiểm sẽ xác định nếu mục được thêm vào hay không. Sự kiện sẽ chỉ được thêm vào nếu Trust= = "tin cậy".

Trustđiểm được xác định bởi SPF, các thuộc tính Mkim hoặc Nhmarc, nằm trong phần đầu thư.

Để xem các thuộc tính sau:

**Outlook trên máy tính**

- Mở mục
- Thuộc tính > tệp-> tiêu đề Internet

hay

**MFCMapi**

- Dẫn hướng đến mục trong hộp thư đến
- Tìm PR_TRANSPORT_MESSAGE_HEADERS_W

Những thuộc tính này được xác định và ghi lại trong quá trình vận chuyển và định tuyến. Để khắc phục sự cố thêm, bạn có thể cần phải theo dõi với hỗ trợ truyền tải về các lỗi trong SPF, MKIM và. hoặc TMARC.