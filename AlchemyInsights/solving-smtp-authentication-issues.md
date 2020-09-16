---
title: Giải quyết các sự cố xác thực SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738011"
---
# <a name="solving-smtp-authentication-issues"></a>Giải quyết các sự cố xác thực SMTP

Nếu bạn đang gặp phải lỗi 5.7.57 hoặc 5.7.3 khi tìm cách gửi email SMTP và xác thực bằng một máy khách hoặc ứng dụng, có một vài điều bạn nên kiểm tra:

- Việc gửi SMTP được xác thực có thể bị vô hiệu hóa trong đối tượng thuê của bạn hoặc trên hộp thư mà bạn đang cố gắng sử dụng (kiểm tra cả hai thiết đặt). Để đọc thêm, hãy xem [bật hoặc tắt trình gửi SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)được xác thực.

- Kiểm tra xem [mặc định bảo mật Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) được bật cho đối tượng thuê của bạn hay không; Nếu được kích hoạt, xác thực SMTP bằng cách dùng xác thực cơ bản (còn được gọi là di sản; điều này sẽ sử dụng tên người dùng và mật khẩu) sẽ không thành công.
