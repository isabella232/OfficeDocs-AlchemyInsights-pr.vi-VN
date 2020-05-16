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
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="8b71e-102">Giải quyết vấn đề xác thực SMTP</span><span class="sxs-lookup"><span data-stu-id="8b71e-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="8b71e-103">Nếu bạn đang nhận được lỗi 5.7.57 hoặc 5.7.3 khi cố gắng để gửi email SMTP và xác thực với một khách hàng hoặc ứng dụng, có một vài điều bạn nên kiểm tra:</span><span class="sxs-lookup"><span data-stu-id="8b71e-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="8b71e-104">Xác thực SMTP gửi có thể bị vô hiệu hoá trong thuê của bạn hoặc trên hộp thư mà bạn đang sử dụng (kiểm tra cả hai cài đặt).</span><span class="sxs-lookup"><span data-stu-id="8b71e-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="8b71e-105">Để đọc thêm, xem [kích hoạt hoặc vô hiệu hoá xác thực khách SMTP gửi](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span><span class="sxs-lookup"><span data-stu-id="8b71e-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="8b71e-106">Kiểm tra xem [mặc định bảo mật Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) được kích hoạt cho đối tượng thuê của bạn; Nếu bật, xác thực SMTP bằng cách sử dụng xác thực cơ bản (còn được gọi là di sản; điều này sẽ sử dụng tên người dùng và mật khẩu) sẽ thất bại.</span><span class="sxs-lookup"><span data-stu-id="8b71e-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
