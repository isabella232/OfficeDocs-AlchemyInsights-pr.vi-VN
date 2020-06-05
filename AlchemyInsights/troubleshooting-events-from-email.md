---
title: Khắc phục sự kiện từ email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569398"
---
# <a name="troubleshooting-events-from-email"></a>Khắc phục sự kiện từ email

1. Kiểm tra tính năng được kích hoạt cho hộp thư: **nhận-EventsFromEmailConfiguration <mailbox> -Identity**

2. Sau đó nhìn vào các ' sự kiện từ email ' Nhật ký **xuất khẩu-Mailboxchẩn Sticlogs <mailbox> -cấu phần timeprofile**

3. Trong Nhật ký "sự kiện từ email", tìm InternetMessageId phù hợp với mục trong hộp thư.  

4. TrustScore xác định nếu mục được thêm vào hay không. Sự kiện sẽ chỉ được thêm vào nếu TrustScore = "tin cậy".

TrustScore được xác định bởi SPF, DKIM hoặc dMarc thuộc tính, trong tiêu đề thư.

Để xem các tính này:

**Máy tính để bàn Outlook**

- Mở mục
- Tệp-> Properties-> tiêu đề Internet

Hoặc

**MFCMapi**

- Điều hướng đến mục trong hộp thư đến
- Tìm kiếm PR_TRANSPORT_MESSAGE_HEADERS_W

Các tính này được xác định và ghi lại trong quá trình vận chuyển và định tuyến. Để khắc phục sự cố thêm, bạn có thể cần phải theo dõi hỗ trợ truyền tải về các lỗi trong SPF, DKIM và. hoặc DMARC.