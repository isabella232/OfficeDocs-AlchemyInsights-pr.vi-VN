---
title: Sự cố với mã thông báo
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
ms.openlocfilehash: a4e99f1f80df601ddf53498d9a8323790fc52a50b2e067f17429da0bf6a03c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067466"
---
# <a name="issues-with-tokens"></a>Sự cố với mã thông báo

Để quản lý các vấn đề liên quan đến mã thông báo, bạn có thể thực hiện các bước sau đây:

1. Bạn có thể chỉ định thời hạn của quyền truy nhập, ID hoặc mã thông báo SAML do người phát hành Nền tảng định danh Microsoft. Bạn có thể đặt thời hạn mã thông báo cho tất cả các ứng dụng trong tổ chức của bạn, cho ứng dụng nhiều đối tượng thuê (nhiều tổ chức) hoặc cho một dịch vụ chính cụ thể trong tổ chức của bạn. Để biết thêm thông tin, hãy [xem mục Thời hạn mã thông báo có thể cấu hình Nền tảng định danh Microsoft (bản xem trước).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
2. Mã thông báo Access cho phép máy khách gọi an toàn các API web được bảo vệ và được các API web sử dụng để thực hiện xác thực và định quyền. Theo đặc tả OAuth, mã thông báo truy nhập là các chuỗi mờ đục mà không có định dạng tập hợp - một số nhà cung cấp định danh (IDP) sử dụng ID, những nhà cung cấp khác sử dụng blob được mã hóa. Trường Nền tảng định danh Microsoft dùng nhiều định dạng mã thông báo truy nhập khác nhau, tùy thuộc vào cấu hình của API chấp nhận mã thông báo. Để tìm hiểu cách API của bạn có thể xác thực và sử dụng các khiếu nại bên trong một mã thông báo truy nhập, hãy [xem Nền tảng định danh Microsoft mã thông báo truy nhập](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Thư viện Xác thực Của Microsoft (MSAL) hỗ trợ một số dòng xác thực để sử dụng trong các kịch bản ứng dụng khác nhau. Để biết thêm thông tin, [hãy xem Dòng xác thực](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Có thể sử dụng cấp mã ủy quyền OAuth 2.0 trong các ứng dụng được cài đặt trên thiết bị để có quyền truy nhập vào các tài nguyên được bảo vệ, chẳng hạn như các API web. Bằng cách sử dụng Nền tảng định danh Microsoft thực thi OAuth 2.0, bạn có thể thêm quyền truy nhập đăng nhập và API vào các ứng dụng dành cho thiết bị di động và máy tính. Xem Nền tảng định danh Microsoft và dòng mã ủy quyền [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) để biết cách lập trình trực tiếp với giao thức trong ứng dụng của bạn, bằng cách sử dụng bất cứ ngôn ngữ nào.
5. OpenID Kết nối (OIDC) là giao thức xác thực được xây dựng trên OAuth 2.0 mà bạn có thể sử dụng để đăng nhập bảo mật người dùng vào một ứng dụng. Khi bạn sử dụng cách triển Nền tảng định danh Microsoft của điểm cuối OpenID Kết nối, bạn có thể thêm quyền truy nhập đăng nhập và API vào các ứng dụng của mình. Nền tảng định danh Microsoft và giao thức [Kết nối OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) cho thấy cách thực hiện việc này độc lập với ngôn ngữ và mô tả cách gửi và nhận thư HTTP mà không sử dụng bất kỳ thư viện mã nguồn mở nào của Microsoft.
    - Điểm cuối UserInfo là một phần của tiêu chuẩn OIDC, được thiết kế để trả về các khiếu nại về người dùng đã xác thực. Để biết thêm thông tin, [hãy Nền tảng định danh Microsoft điểm cuối UserInfo.](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)
    - Mẫu Gọi web API trong ứng dụng web bằng Azure AD và [OpenID Kết nối](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) cho thấy cách xây dựng một ứng dụng web MVC sử dụng Azure AD để đăng nhập bằng giao thức OpenID Kết nối, rồi gọi đến API web theo danh tính người dùng đã đăng nhập bằng mã thông báo có được thông qua OAuth 2.0. Mẫu này sử dụng OpenID Kết nối ASP .Net OWIN middleware và ADAL .Net.
6. [Cấu](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) hình một ứng dụng để xuất hiện một API web - Trong khởi động nhanh này, bạn đăng ký một API web với Nền tảng định danh Microsoft và cung cấp nó cho các ứng dụng máy khách bằng cách thêm một phạm vi ví dụ. Bằng cách đăng ký API web của bạn và giới hạn thông qua các phạm vi, bạn có thể cung cấp quyền truy nhập dựa trên quyền vào các tài nguyên của nó cho người dùng được ủy quyền và ứng dụng máy khách truy nhập API của bạn.
7. Trong Azure Active Directory B2C (Azure AD B2C), dòng thông tin xác thực mật khẩu chủ sở hữu tài nguyên (ROPC) là dòng xác thực chuẩn OAuth. Trong dòng này, một ứng dụng, còn được gọi là bên tin dùng, trao đổi thông tin xác thực hợp lệ cho mã thông báo. Thông tin xác thực bao gồm ID người dùng và mật khẩu. Các mã thông báo được trả về là mã thông báo ID, mã thông báo truy nhập và mã thông báo làm mới. Để biết thêm thông tin, hãy xem mục Thiết lập dòng thông tin xác thực mật khẩu chủ sở hữu [tài Azure Active Directory B2C.](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow) 

