---
title: lỗi 1554 Winsock 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698884"
---
# <a name="winsock-error-10061"></a>Lỗi Winsock 10061

Mã lỗi này có nghĩa là Microsoft không thể thiết lập một ổ cắm TCP (kết nối) với máy chủ đích. Nguyên nhân có thể nhất của lỗi này là sự cố với cấu hình tường lửa của bạn. Để khắc phục sự cố, hãy kiểm tra các thiết đặt sau:

- Xác nhận cấu hình tường lửa của bạn với thông tin trong [URL Microsoft 365 và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Nếu lỗi cụ thể với Exchange Online Protection (EOP), bạn nên trước đó đã được thông báo đến một thay đổi đối với các [địa chỉ IP của Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Xác minh rằng nhà cung cấp dịch vụ Internet (ISP của bạn) không ngăn không cho cổng.

- Xác nhận thiết đặt máy chủ lưu trữ và đích thông minh trong đường kết nối của bạn.

Lưu ý rằng Microsoft 365 không chặn kết nối *đến* theo cách này.
