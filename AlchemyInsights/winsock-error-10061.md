---
title: Lỗi Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083252"
---
# <a name="winsock-error-10061"></a>Lỗi Winsock 10061

Mã lỗi này có nghĩa là Microsoft không thể thiết lập khe (kết nối) TCP với máy chủ đích. Nguyên nhân thường gặp nhất của lỗi này là do cấu hình tường lửa của bạn có vấn đề. Để khắc phục sự cố, hãy kiểm tra các thiết đặt sau:

- Xác minh cấu hình tường lửa của bạn với [thông tin Microsoft 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Nếu lỗi này dành riêng cho người Exchange Online Protection (EOP), trước đó bạn sẽ được thông báo về việc thay đổi [địa Exchange Online Protection IP mới.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Xác nhận rằng Nhà cung cấp Dịch vụ Internet (ISP) của bạn không chặn cổng.

- Xác nhận thiết đặt máy chủ thông minh và máy chủ đích trong các đường kết nối của bạn.

Lưu ý rằng Microsoft 365 chặn các kết *nối đến* theo cách này.
