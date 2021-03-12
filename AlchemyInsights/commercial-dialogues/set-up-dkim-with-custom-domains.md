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
# <a name="set-up-dkim-with-custom-domains"></a>Thiết lập các hàm MKIM với tên miền tùy chỉnh

Bạn phải phát hành hai bản ghi CNAME cho mỗi tên miền tùy chỉnh trong DNS. Để thực hiện điều này, hãy dùng định dạng sau:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **Domainguid** là văn bản ở bên trái của **. mail.Protection.Outlook.com** trong bản ghi MX tùy chỉnh cho tên miền tùy chỉnh (ví dụ: contoso-com cho tên miền **contoso.com**). **Initialdomain** là tên miền mà bạn đã sử dụng khi đăng ký Office 365 (ví dụ, **contoso.onmicrosoft.com**).

Để biết thêm thông tin về bản ghi DNS, hãy xem [tạo bản ghi DNS tại bất kỳ nhà cung cấp lưu trữ DNS nào cho Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).