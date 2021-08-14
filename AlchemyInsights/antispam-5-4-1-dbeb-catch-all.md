---
title: AntiSpam 5.4.1 DBEB bao trùm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932299"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Khắc phục sự cố chuyển phát cho mã lỗi 550 5.4.1 Relay Access Denied

Sự cố này xảy ra khi [kiểm tra xem một địa chỉ email có](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) hợp lệ không để tránh bị trả lại khi nhập mạng Microsoft. Hãy thử cách sau:

1. Xác định xem sự cố cụ thể với toàn bộ tên miền hay một địa chỉ email duy nhất:
    - Toàn bộ miền: Đôi khi miền cần được đồng bộ hóa; hãy [thử thiết đặt miền thành Nội bộ rồi quay lại Có thẩm quyền.](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - Địa chỉ email đơn: Đôi khi địa chỉ cần được đồng bộ hóa; thay đổi địa chỉ proxy smtp và sau đó thay đổi lại địa chỉ proxy đó có thể giúp ích.
2. Xác định xem vấn đề này cụ thể đối với một nhóm hay thư mục công cộng. Đối với một số kiểu đối tượng, các đối tượng có thể cần được tạo thủ công trong Azure Active Directory.

Nếu bạn cần trợ giúp thêm, vui lòng mở thẻ hỗ trợ và chỉ định phạm vi của sự cố (bao gồm loại đối tượng bạn đang gửi đến) để chúng tôi có thể trợ giúp bạn tốt hơn.