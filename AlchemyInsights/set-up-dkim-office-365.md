---
title: Thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108578"
---
# <a name="setup-dkim"></a>Thiết lập DKIM

Hướng dẫn đầy đủ để đặt cấu hình DKIM cho tên miền riêng Microsoft 365 tại [đây.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Đối **với** mỗi tên miền riêng, bạn cần tạo hai bản ghi **CNAME** DKIM tại dịch vụ lưu trữ DNS của tên miền (thường là cơ quan đăng ký tên miền). Ví dụ: contoso.com và fourthcoffee.com yêu cầu bốn bản ghi CNAME DKIM: hai bản ghi cho contoso.com và hai bản ghi cho fourthcoffee.com.

   Bản ghi CNAME DKIM cho mỗi **tên miền riêng** sử dụng các định dạng sau đây:

   - **Tên máy chủ:**`selector1._domainkey.<CustomDomain>`

     **Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Tên máy chủ:**`selector2._domainkey.<CustomDomain>`

     **Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> là văn bản ở bên trái trong bản ghi MX tùy chỉnh cho tên miền riêng `.mail.protection.outlook.com` (ví dụ, `contoso-com` đối với tên miền contoso.com). \<InitialDomain\>là miền mà bạn đã sử dụng khi đăng ký Microsoft 365 đó (ví dụ: miền contoso.onmicrosoft.com).

2. Sau khi bạn đã tạo các bản ghi CNAME cho tên miền riêng của mình, hãy hoàn thành các hướng dẫn sau đây:

   a. [đăng nhập vào Microsoft 365 bằng tài](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) khoản cơ quan hoặc trường học của bạn.

   b. Chọn biểu tượng công cụ khởi động ứng dụng ở góc trên bên trái và chọn Người **quản trị.**

   c. Trong dẫn hướng phía dưới bên trái, hãy bung **rộng Quản** trị và **Exchange.**

   d. Đi tới  >  **DKIM Bảo vệ**.

   e. Chọn miền, rồi chọn **Bật cho** Ký thư cho miền này với chữ **ký DKIM.** Lặp lại bước này cho từng tên miền riêng.
