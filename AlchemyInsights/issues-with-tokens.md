---
title: Các vấn đề với thẻ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917212"
---
# <a name="issues-with-tokens"></a>Các vấn đề với thẻ

Để quản lý các vấn đề liên quan đến thẻ, bạn có thể thực hiện các bước sau đây:

1. Bạn có thể xác định tuổi thọ của một mã thông báo Access, ID hoặc SAML do Microsoft Identity Platform phát hành. Bạn có thể đặt các hạn token cho tất cả các ứng dụng trong tổ chức của mình, cho một ứng dụng nhiều đối tượng thuê (nhiều tổ chức) hoặc đối với một hiệu trưởng dịch vụ cụ thể trong tổ chức của bạn. Để biết thêm thông tin, hãy xem [cấu hình hạn token trong Microsoft Identity Platform (bản xem trước)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Truy nhập thẻ cho phép khách hàng sử dụng các API web được bảo vệ an toàn và được các API web dùng để thực hiện xác thực và ủy quyền. Theo đặc tả OAuth, thẻ Access là các chuỗi mờ mà không có định dạng đặt-một số nhà cung cấp danh tính (IDPs) sử dụng GUID, những người khác sử dụng các đốm màu đã mã hóa. Nền tảng Microsoft Identity sử dụng một loạt các định dạng mã thông báo Access, tùy thuộc vào cấu hình của API chấp nhận mã thông báo. Để tìm hiểu cách API của bạn có thể xác thực và sử dụng các tuyên bố bên trong mã thông báo Access, hãy xem [thẻ truy nhập Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Thư viện xác thực Microsoft (MSAL) hỗ trợ một số dòng xác thực để sử dụng trong các kịch bản ứng dụng khác nhau. Để biết thêm thông tin, hãy xem [dòng xác thực](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Cấp phép mã OAuth 2,0 có thể được sử dụng trong các ứng dụng được cài đặt trên một thiết bị để truy nhập vào các tài nguyên được bảo vệ, chẳng hạn như các API web. Sử dụng Microsoft Identity Platform thực hiện của OAuth 2,0, bạn có thể thêm đăng nhập và truy nhập API vào ứng dụng di động và máy tính bàn của bạn. Xem [nền tảng Microsoft Identity và dòng mã ủy quyền OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) để làm thế nào để chương trình trực tiếp chống lại giao thức trong ứng dụng của bạn, sử dụng bất kỳ ngôn ngữ nào.
5. Kết nối OpenID (OIDC) là một giao thức xác thực được tích hợp trên máy tính OAuth 2,0 mà bạn có thể sử dụng để đăng nhập an toàn trong một ứng dụng. Khi bạn sử dụng tính năng triển khai kết nối OpenID Identity Platform của Microsoft, bạn có thể thêm đăng nhập và truy nhập API vào ứng dụng của mình. [Giao thức Microsoft Identity Platform và OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) cho biết cách làm điều này độc lập với ngôn ngữ và mô tả cách gửi và nhận thư http mà không cần sử dụng bất kỳ thư viện nguồn mở nào của Microsoft.
    - Điểm cuối UserInfo là một phần của tiêu chuẩn OIDC, được thiết kế để trả về tuyên bố về người dùng đã xác thực. Để biết thêm thông tin, hãy xem điểm [cuối của Microsoft Identity Platform UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - Tính năng [gọi cho một API web trong một ứng dụng web bằng cách sử dụng AZURE AD và OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) mẫu cho biết cách xây dựng một ứng dụng web MVC sử dụng Azure AD để đăng nhập bằng cách sử dụng giao thức kết nối OpenID, rồi gọi đến một API web bên dưới định danh của người dùng đã đăng nhập bằng cách sử dụng thẻ thu được qua oauth 2,0. Mẫu này sử dụng kết nối OpenID ASP .net OWIN middleware và ADAL .net.
6. [Cấu hình ứng dụng để hiển thị một API web](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -trong bắt đầu nhanh này, bạn đăng ký một API web với nền tảng định danh Microsoft và vạch trần nó vào ứng dụng máy khách bằng cách thêm phạm vi ví dụ. Bằng cách đăng ký API web của bạn và phơi bày thông qua phạm vi, bạn có thể cung cấp quyền truy nhập dựa trên quyền đối với các tài nguyên cho người dùng và ứng dụng khách cho phép truy nhập API của bạn.
7. Trong Azure Active Directory B2C (Azure AD B2C), dòng thông tin đăng ký mật khẩu của chủ sở hữu tài nguyên (ROPC) là dòng xác thực chuẩn OAuth. Trong dòng này, một ứng dụng, còn được gọi là đảng, hãy trao đổi thông tin xác thực hợp lệ cho thẻ. Chứng danh bao gồm ID người dùng và mật khẩu. Thẻ được trả về là một mã thông báo ID, mã thông báo Access và một mã thông báo làm mới. Để biết thêm thông tin, hãy xem mục [thiết lập dòng chứng danh của chủ sở hữu tài nguyên trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

