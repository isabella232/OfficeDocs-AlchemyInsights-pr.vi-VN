---
title: Theo dõi quyền truy nhập InTune có điều kiện
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428312"
---
# <a name="monitor-intune-conditional-access"></a>Theo dõi quyền truy nhập InTune có điều kiện

Người dùng được mục tiêu với quyền truy nhập có điều kiện sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập của tổ chức bạn. Để giải quyết, chúng tôi khuyên bạn nên một hoặc nhiều giải pháp sau đây:

1. Nếu thiết bị được cho là đã đăng ký, hãy tư vấn cho người dùng để đi đến ứng dụng cổng thông tin công ty và xác minh rằng nó sẽ xuất hiện trong cổng thông tin công ty. Nếu không, người dùng phải đăng ký thiết bị.
1. Trong cổng thông tin Azure, đi đến  >  **tuân thủ thiết bị** InTune. 
1. Để xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là tuân thủ, bên dưới **giám sát**, hãy bấm **tuân thủ thiết bị**.
1. Trong cổng thông tin Azure, đi đến  >  **tuân thủ thiết bị** InTune. Bên dưới **quản lý,** bấm vào **chính sách**. Trong danh sách các chính sách tuân thủ, hãy xác nhận hồ sơ được gán cho thiết bị của người dùng. Nếu không có hồ sơ nào được phân công, thì InTune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.
1. Chỉnh sửa nhiệm vụ truy nhập có điều kiện của người dùng.
1. Trong cổng thông tin Azure, dẫn hướng đến các chính sách truy nhập **InTune** có điều  >  **kiện**  >  , hãy chọn một chính sách từ danh sách và bấm vào **người dùng và nhóm**.
1. Để nhắm đến một chính sách nhất định tại một ai đó, hãy thêm họ vào **danh sách bao gồm**. Để đảm bảo rằng một người được bỏ qua khỏi chính sách, hãy thêm họ vào **danh sách loại trừ**.

**Liên kết hữu ích:**

- [Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Chính sách khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Giám sát việc tuân thủ thiết bị InTune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Các bước này chỉ hữu ích trong việc khắc phục sự cố truy nhập các tính năng Azure Active Directory có điều kiện. Cũng có thể để cách ly thiết bị chặn truy nhập email với chính sách Exchange. Có thể tìm hiểu thêm thông tin về quản lý thiết bị Exchange [**tại đây**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).
