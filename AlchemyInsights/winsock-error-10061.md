---
title: 1554 Winsock lỗi 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766191"
---
# <a name="winsock-error-10061"></a>Winsock lỗi 10061

Mã lỗi này có nghĩa là Microsoft không thể thiết lập một ổ cắm TCP (kết nối) với máy chủ đích. Nguyên nhân có thể gây ra lỗi này là một vấn đề với cấu hình tường lửa của bạn. Để khắc phục sự cố, hãy kiểm tra các cài đặt này:

- Xác minh cấu hình tường lửa của bạn với thông tin trong [Microsoft 365 URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Nếu lỗi cụ thể để bảo vệ trực tuyến Exchange (EOP), bạn phải được thông báo trước đó để thay đổi [địa chỉ IP bảo vệ trực tuyến Exchange](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Xác minh rằng nhà cung cấp dịch vụ Internet (ISP) của bạn không chặn cổng.

- Kiểm tra các máy chủ thông minh và mục tiêu cài đặt trong kết nối của bạn.

Lưu ý rằng Microsoft 365 không chặn các kết nối *đến* theo cách này.
