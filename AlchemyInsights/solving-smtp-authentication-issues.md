---
title: Giải quyết vấn đề xác thực SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 814c49e8e65966a0c9f927b1f7bfb03d3dc3d637
ms.sourcegitcommit: 0e43e19448705f151846e9e9e1e0f47e12938fdf
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/15/2020
ms.locfileid: "44264567"
---
# <a name="solving-smtp-authentication-issues"></a>Giải quyết vấn đề xác thực SMTP

Nếu bạn đang nhận được lỗi 5.7.57 hoặc 5.7.3 khi cố gắng để gửi email SMTP và xác thực với một khách hàng hoặc ứng dụng, có một vài điều bạn nên kiểm tra:

- Xác thực SMTP gửi có thể bị vô hiệu hoá trong thuê của bạn hoặc trên hộp thư mà bạn đang sử dụng (kiểm tra cả hai cài đặt). Để đọc thêm, xem [kích hoạt hoặc vô hiệu hoá xác thực khách SMTP gửi](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).

- Kiểm tra xem [mặc định bảo mật Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) được kích hoạt cho đối tượng thuê của bạn; Nếu bật, xác thực SMTP bằng cách sử dụng xác thực cơ bản (còn được gọi là di sản; điều này sẽ sử dụng tên người dùng và mật khẩu) sẽ thất bại.
