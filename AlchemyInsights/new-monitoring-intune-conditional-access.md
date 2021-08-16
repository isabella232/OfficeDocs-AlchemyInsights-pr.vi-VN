---
title: Giám sát Quyền truy cập có điều kiện của Intune
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
ms.openlocfilehash: 7f30202ff0a5b9475393cf26c0506bd6bec24f3d378052f24ebf7f327cf84689
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025524"
---
# <a name="monitor-intune-conditional-access"></a>Giám sát Quyền truy cập có điều kiện của Intune

Người dùng được quyền truy nhập có điều kiện hướng tới sẽ nhận được email thông báo nếu họ không đáp ứng các yêu cầu truy nhập từ tổ chức của bạn. Để giải quyết, chúng tôi đề xuất một hoặc nhiều giải pháp sau đây:

1. Nếu thiết bị được giả định là đã đăng ký, hãy đề nghị người dùng truy nhập ứng dụng Company Portal và xác minh xem thiết bị có xuất hiện trong danh Company Portal. Nếu thiết bị không xuất hiện, người dùng phải đăng ký thiết bị.
1. Trong Cổng thông tin Azure, đi tới **Tuân thủ thiết bị Intune**  >  . 
1. Để xem báo cáo tuân thủ thiết bị của bạn để xác minh rằng thiết bị của người dùng được đánh dấu là đã tuân thủ, bên dưới Giám sát **,** bấm vào Tuân thủ **thiết bị**.
1. Trong Cổng thông tin Azure, đi tới **Tuân thủ thiết bị Intune**  >  . Bên dưới **Quản lý,** bấm vào **Chính sách.** Trong danh sách các chính sách tuân thủ, hãy xác minh rằng thiết bị người dùng của bạn đã được gán hồ sơ. Nếu chưa gán hồ sơ, Intune sẽ không thể xác nhận trạng thái tuân thủ của thiết bị.
1. Chỉnh sửa nội dung gán quyền truy nhập có điều kiện của người dùng.
1. Trong cổng thông tin Azure, dẫn hướng đến Chính sách truy nhập có điều kiện **của Intune**, chọn một chính sách từ danh  >    >  sách, rồi bấm vào **Người dùng và nhóm.**
1. Để hướng một chính sách nhất định tới đối tượng nào đó, hãy thêm người đó vào **danh sách Bao gồm.** Để đảm bảo loại bỏ một người khỏi chính sách, hãy thêm người đó vào danh sách **Loại trừ**.

**Các liên kết hữu ích:**

- [Tổng quan về tuân thủ thiết bị](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Khắc phục sự cố CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Chính sách khắc phục sự cố](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Giám sát sự tuân thủ của thiết bị Intune](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> Các bước này chỉ hữu ích trong việc khắc phục sự cố về Azure Active Directory năng Truy nhập có điều kiện. Cũng có thể cách ly một thiết bị chặn quyền truy nhập email của thiết bị đó với chính Exchange bạn. Có thể tìm thấy thêm thông tin Exchange lý thiết bị tại [**đây.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
