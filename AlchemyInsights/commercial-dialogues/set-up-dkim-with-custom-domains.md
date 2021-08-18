---
title: Thiết lập DKIM với tên miền riêng
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
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332329"
---
# <a name="set-up-dkim-with-custom-domains"></a>Thiết lập DKIM với tên miền riêng

Bạn phải phát hành hai bản ghi CNAME cho mỗi tên miền riêng trong DNS. Để thực hiện điều này, hãy dùng định dạng sau đây:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Lưu** ý: **DomainGUID** là văn bản ở bên trái của **.mail.protection.outlook.com** trong bản ghi MX tùy chỉnh cho miền tùy chỉnh (ví dụ: contoso-com cho miền **contoso.com).** **InitialDomain là** tên miền mà bạn đã sử dụng khi đăng ký Office 365 (ví dụ, **contoso.onmicrosoft.com).**

Để biết thêm thông tin về bản ghi DNS, hãy [xem Tạo bản ghi DNS tại nhà cung cấp lưu trữ DNS bất kỳ Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)