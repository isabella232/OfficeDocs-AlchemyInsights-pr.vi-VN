---
title: Mã lỗi 550 5.7.501 truy cập bị từ chối, lạm dụng thư rác phát hiện
ms.author: chrisda
author: chrisda
ms.date: 6/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 545cab07cc7c49def849be20bb6363da228a5393
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36740163"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="cb0bf-102">550 5.7.501 truy cập bị từ chối, lạm dụng thư rác phát hiện</span><span class="sxs-lookup"><span data-stu-id="cb0bf-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="cb0bf-103">Thông thường, thư này xảy ra khi người dùng gửi thư điện tử từ địa chỉ IP bằng cách sử dụng tên miền *. onmicrosoft.com* ban đầu được gán cho người thuê mới trong Office 365.</span><span class="sxs-lookup"><span data-stu-id="cb0bf-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Office 365.</span></span> <span data-ttu-id="cb0bf-104">Cách dễ nhất để giải quyết vấn đề này là:</span><span class="sxs-lookup"><span data-stu-id="cb0bf-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="cb0bf-105">[Thêm tên miền cho đối tượng thuê của bạn](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="cb0bf-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="cb0bf-106">[Thay đổi địa chỉ email chính của người dùng](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) thành miền tùy chỉnh mới mà bạn vừa thêm.</span><span class="sxs-lookup"><span data-stu-id="cb0bf-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
