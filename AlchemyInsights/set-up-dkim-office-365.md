---
title: Thiết lập TKIM
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
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808729"
---
# <a name="setup-dkim"></a>Thiết lập TKIM

Hướng dẫn đầy đủ để đặt cấu hình cho các tên miền tùy chỉnh trong Microsoft 365 ở [đây](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. Đối với **mỗi** tên miền tùy chỉnh, bạn cần phải tạo **hai** bản ghi CNAME trên máy chủ lưu trữ DNS của tên miền của bạn (thường là cơ quan đăng ký tên miền). Ví dụ, contoso.com và fourthcoffee.com yêu cầu bốn bản ghi CNAME được tạo: hai cho contoso.com và hai đối với fourthcoffee.com.

   Bản ghi CNAME của **MKIM cho mỗi** tên miền tùy chỉnh sử dụng các định dạng sau:

   - **Tên máy chủ**: `selector1._domainkey.<CustomDomain>`

     **Trỏ tới địa chỉ hoặc giá trị**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Tên máy chủ**: `selector2._domainkey.<CustomDomain>`

     **Trỏ tới địa chỉ hoặc giá trị**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> là văn bản ở bên trái `.mail.protection.outlook.com` trong bản ghi MX tùy chỉnh cho tên miền tùy chỉnh (ví dụ: `contoso-com` đối với tên miền contoso.com). \<InitialDomain\> là tên miền mà bạn đã sử dụng khi đăng ký Microsoft 365 (ví dụ, contoso.onmicrosoft.com).

2. Sau khi bạn đã tạo bản ghi CNAME cho tên miền riêng của mình, hãy hoàn thành các hướng dẫn sau đây:

   một. [đăng nhập vào Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) bằng tài khoản cơ quan hoặc trường học của bạn.

   b. Chọn biểu tượng công cụ khởi động ứng dụng ở phía trên bên trái, rồi chọn người **quản trị**.

   c's. Trong dẫn hướng phía dưới bên trái, hãy bung rộng **quản trị** và chọn **Exchange**.

   dâm. Đi đến **bảo vệ**  >  **d**.

   e's. Chọn tên miền và sau đó chọn **bật** cho **tin nhắn đăng nhập cho tên miền này với chữ ký**trong dấu kim. Lặp lại bước này cho mỗi tên miền tùy chỉnh.
