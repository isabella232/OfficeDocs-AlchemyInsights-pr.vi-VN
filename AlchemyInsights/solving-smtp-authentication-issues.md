---
title: Giải quyết các sự cố xác thực SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826437"
---
# <a name="solving-smtp-authentication-issues"></a>Giải quyết các sự cố xác thực SMTP

Nếu bạn đang gặp phải lỗi 5.7.57 hoặc 5.7.3 khi tìm cách gửi email SMTP và xác thực bằng một máy khách hoặc ứng dụng, có một vài điều bạn nên kiểm tra:

- Việc gửi SMTP được xác thực có thể bị vô hiệu hóa trong đối tượng thuê của bạn hoặc trên hộp thư mà bạn đang cố gắng sử dụng (kiểm tra cả hai thiết đặt). Để đọc thêm, hãy xem [bật hoặc tắt trình gửi SMTP](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)được xác thực.

- Kiểm tra xem [mặc định bảo mật Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) được bật cho đối tượng thuê của bạn hay không; Nếu được kích hoạt, xác thực SMTP bằng cách dùng xác thực cơ bản (còn được gọi là di sản; điều này sẽ sử dụng tên người dùng và mật khẩu) sẽ không thành công.
