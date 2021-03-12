---
title: Thiết lập các hàm MKIM với tên miền tùy chỉnh
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747631"
---
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="b859b-102">Thiết lập các hàm MKIM với tên miền tùy chỉnh</span><span class="sxs-lookup"><span data-stu-id="b859b-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="b859b-103">Bạn phải phát hành hai bản ghi CNAME cho mỗi tên miền tùy chỉnh trong DNS.</span><span class="sxs-lookup"><span data-stu-id="b859b-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="b859b-104">Để thực hiện điều này, hãy dùng định dạng sau:</span><span class="sxs-lookup"><span data-stu-id="b859b-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="b859b-105">**Domainguid** là văn bản ở bên trái của **. mail.Protection.Outlook.com** trong bản ghi MX tùy chỉnh cho tên miền tùy chỉnh (ví dụ: contoso-com cho tên miền **contoso.com**).</span><span class="sxs-lookup"><span data-stu-id="b859b-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="b859b-106">**Initialdomain** là tên miền mà bạn đã sử dụng khi đăng ký Office 365 (ví dụ, **contoso.onmicrosoft.com**).</span><span class="sxs-lookup"><span data-stu-id="b859b-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="b859b-107">Để biết thêm thông tin về bản ghi DNS, hãy xem [tạo bản ghi DNS tại bất kỳ nhà cung cấp lưu trữ DNS nào cho Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="b859b-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>