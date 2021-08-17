---
title: Khắc phục sự kiện từ Email
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105374"
---
# <a name="troubleshooting-events-from-email"></a>Khắc phục sự kiện từ Email

1. Xác minh tính năng được bật cho hộp thư: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Sau đó, hãy xem nhật ký 'Sự kiện từ Email' **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Trong nhật ký 'Sự kiện từ Email', hãy tìm InternetMessageId khớp với mục trong hộp thư.  

4. TrustScore sẽ xác định mục đó đã được thêm vào hay chưa. Sự kiện sẽ chỉ được thêm nếu TrustScore = "Đáng tin cậy".

Điểm tin cậy được xác định bởi các thuộc tính SPF, Dkim hoặc Dmarc, vốn nằm trong Thông tin Thư.

Để xem các thuộc tính này:

**Màn hình Outlook**

- Mở mục
- File -> Properties -> Internet Headers

hoặc

**MFCMapi**

- Dẫn hướng đến mục trong hộp thư đến
- Tìm kiếm PR_TRANSPORT_MESSAGE_HEADERS_W

Những thuộc tính này được xác định và ghi lại trong quá trình truyền và định tuyến. Để khắc phục sự cố thêm, bạn có thể cần theo dõi với Bộ trợ giúp Truyền dẫn về các lỗi trong SPF, DKIM và.hoặc DMARC.