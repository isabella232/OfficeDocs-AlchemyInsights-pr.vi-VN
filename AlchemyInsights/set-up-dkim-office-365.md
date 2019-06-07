---
title: Thiết lập DKIM trong Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765561"
---
# <a name="setup-dkim-in-office-365"></a>Thiết lập DKIM trong Office 365

Hướng dẫn đầy đủ cho các cấu hình DKIM cho các lĩnh vực tùy chỉnh trong Office 365 là [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Cho **mỗi** tên miền tuỳ chỉnh, bạn cần để tạo ra **hai** DKIM bản ghi CNAME tại tên miền của bạn dịch vụ lưu trữ DNS (thông thường, nhà cung cấp miền). Ví dụ: contoso.com và fourthcoffee.com yêu cầu bốn ghi DKIM CNAME: hai cho contoso.com và hai cho fourthcoffee.com.

   Bản ghi DKIM CNAME cho **mỗi** tên miền tuỳ chỉnh sử dụng định dạng sau:

   - **Tên máy chủ**:`selector1._domainkey.<CustomDomain>`

     **Điểm đến địa chỉ hoặc giá trị**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Tên máy chủ**:`selector2._domainkey.<CustomDomain>`

     **Điểm đến địa chỉ hoặc giá trị**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> văn bản bên trái của `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh tùy chỉnh tên miền (ví dụ, `contoso-com` cho miền contoso.com). \<InitialDomain\> là tên miền bạn đã sử dụng khi đăng ký Office 365 (ví dụ, contoso.onmicrosoft.com).

2. Sau khi bạn đã tạo bản ghi CNAME cho miền của bạn tùy chỉnh, đầy đủ các hướng dẫn sau:

   một. [Đăng nhập Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) với tài khoản của bạn làm việc hoặc trường học.

   b. Chọn biểu tượng phóng ứng dụng ở trên bên trái và chọn **Admin**.

   c. Điều hướng dưới bên trái, mở rộng các **Admin** và chọn **Exchange**.

   d. Đi để **bảo vệ** > **DKIM**.

   e. Chọn tên miền và sau đó chọn **sử** **ký**thư cho miền này với DKIM chữ ký. Lặp lại bước này cho mỗi tên miền tuỳ chỉnh.
