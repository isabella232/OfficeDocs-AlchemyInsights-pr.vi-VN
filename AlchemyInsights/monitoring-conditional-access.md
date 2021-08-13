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
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975123"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Giám sát Quyền truy nhập có điều kiện để Exchange

Người dùng được quyền truy nhập có điều kiện hướng tới sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập từ tổ chức của bạn. Để giải quyết, chúng tôi đề xuất một hoặc nhiều giải pháp sau đây:

- Nếu thiết bị được giả định là đã đăng ký, hãy đề nghị người dùng truy nhập ứng dụng Company Portal và xác minh xem thiết bị có xuất hiện trong danh Company Portal. Nếu thiết bị không xuất hiện, người dùng nên đăng ký thiết bị.
- Trong Cổng thông tin Azure, đi tới Intune và > Tuân thủ thiết bị. Bên dưới Giám sát, bấm vào Tuân thủ thiết bị. Xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là đã tuân thủ.
- Trong Cổng thông tin Azure, đi tới Intune và > Tuân thủ thiết bị. Bên dưới Quản lý, bấm vào Chính sách. Trong danh sách các chính sách tuân thủ, hãy xác minh rằng thiết bị người dùng của bạn đã được gán hồ sơ. Nếu chưa gán hồ sơ, Intune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.
- Chỉnh sửa nội dung gán quyền truy nhập có điều kiện của người dùng.

1. Trong Cổng thông tin Azure, đi tới Chính sách truy nhập có điều kiện của **Intune**  >    >  .
2. Chọn một chính sách từ danh sách.
3. Bấm Người dùng và nhóm.
4. Để hướng một chính sách nhất định tới đối tượng nào đó, hãy thêm người đó vào danh sách Bao gồm. Để đảm bảo loại bỏ một người khỏi chính sách, thêm người đó vào danh sách Loại trừ.

Các liên kết hữu ích:

[Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)

[Khắc phục sự cố CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Chính sách khắc phục sự cố](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Giám sát sự tuân thủ của thiết bị Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

Lưu ý: các bước này chỉ hữu ích trong việc khắc phục sự cố về Azure Active Directory năng Truy nhập có điều kiện. Cũng có thể cách ly một thiết bị chặn quyền truy nhập email của thiết bị đó với chính Exchange bạn. Thông tin thêm về Exchange quản lý thiết bị cũng có thể tìm thấy [here]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
