---
title: Thiết lập DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645694"
---
# <a name="setup-dkim"></a>Thiết lập DKIM

Hướng dẫn đầy đủ để cấu hình DKIM cho tuỳ chỉnh miền trong Microsoft 365 đang [ở đây](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Đối với **mỗi** miền tùy chỉnh, bạn cần tạo **hai** bản ghi DKIM CNAME tại dịch vụ lưu trữ DNS của miền (thông thường là công ty đăng ký tên miền). Ví dụ, contoso.com và fourthcoffee.com yêu cầu bốn bản ghi DKIM CNAME: hai cho contoso.com và hai cho fourthcoffee.com.

   Bản ghi DKIM CNAME cho **mỗi** miền tùy chỉnh sử dụng các định dạng sau:

   - **Tên máy chủ**:`selector1._domainkey.<CustomDomain>`

     **Điểm đến địa chỉ hoặc giá trị**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Tên máy chủ**:`selector2._domainkey.<CustomDomain>`

     **Điểm đến địa chỉ hoặc giá trị**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> là văn bản bên trái `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh cho miền tùy chỉnh (ví dụ: `contoso-com` đối với miền contoso.com). \<InitialDomain\> là tên miền bạn sử dụng khi bạn đăng ký Microsoft 365 (ví dụ: contoso.onmicrosoft.com).

2. Sau khi bạn đã tạo bản ghi CNAME cho miền tùy chỉnh của mình, hãy hoàn tất các hướng dẫn sau:

   A. [đăng nhập vào Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) bằng tài khoản nơi làm việc hoặc trường học của bạn.

   B. Chọn biểu tượng trình khởi chạy ứng dụng ở góc trên bên trái và chọn **quản trị viên**.

   C. Ở phía dưới bên trái điều hướng, mở rộng **quản trị** và chọn **Exchange**.

   D. Đi đến **bảo vệ** > **DKIM**.

   E. Chọn miền và sau đó chọn **bật** để **ký thư cho miền này bằng chữ ký DKIM**. Lặp lại bước này cho mỗi miền tùy chỉnh.
