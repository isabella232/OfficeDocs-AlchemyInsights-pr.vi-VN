---
title: Giám sát quyền truy nhập có điều kiện
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708696"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Giám sát quyền truy nhập có điều kiện cho Exchange

Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn. Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:

- Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty. Nếu không, người dùng sẽ đăng ký thiết bị.
- Trong cổng thông tin Azure, đi tới InTune > tuân thủ thiết bị. Bên dưới giám sát bấm tuân thủ thiết bị. Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là phù hợp.
- Trong cổng thông tin Azure, đi tới InTune > tuân thủ thiết bị. Bên dưới quản lý, bấm vào chính sách. Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng. Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.
- Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.

1. Trong cổng thông tin Azure, đi tới  >    >  **chính sách** truy nhập InTune có điều kiện.
2. Chọn một chính sách từ danh sách.
3. Bấm vào người dùng và nhóm.
4. Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào danh sách bao gồm. Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào danh sách loại trừ.

Liên kết hữu ích:

[Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)

[Khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Chính sách khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Giám sát việc tuân thủ thiết bị InTune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Lưu ý: các bước sau đây chỉ hữu ích trong việc khắc phục sự cố truy nhập các tính năng Azure Active Directory có điều kiện. Cũng có thể để cách ly thiết bị chặn truy nhập email với chính sách Exchange. Tìm hiểu thêm thông tin về quản lý thiết bị Exchange [ở đây] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
