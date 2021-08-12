---
title: Khắc phục sự cố về OAuth 2.0 và OpenID Kết nối thức
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921065"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Khắc phục sự cố về OAuth 2.0 và OpenID Kết nối thức

Để giải quyết các vấn đề liên quan đến OAuth 2.0 và OpenID Kết nối, hãy thực hiện các bước được đề xuất sau đây:

Tham khảo các bài viết sau đây liên quan đến cấu hình và khắc phục sự cố cho OAuth 2.0 và OpenID Kết nối thức:

- Nền tảng định danh Microsoft và dòng mã ủy quyền [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - Bài viết này mô tả cách lập trình trực tiếp đối với dòng cấp mã **(PKCE)** trong ứng dụng của bạn, bằng bất kỳ ngôn ngữ nào.
- Nền tảng định danh Microsoft và dòng thông tin xác thực máy khách [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Bài viết này mô tả cách lập trình trực tiếp với dòng thông tin xác thực máy khách trong **ứng** dụng của bạn.
- Nền tảng định danh Microsoft và Thông tin xác thực Mật khẩu chủ sở hữu tài nguyên [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - Bài viết này mô tả cách lập trình trực tiếp với dòng **ROPC** trong ứng dụng của bạn.
    - Công cụ Nền tảng định danh Microsoft hỗ trợ ROPC cho đối tượng thuê Azure AD chứ không hỗ trợ tài khoản cá nhân. Điều này có nghĩa là bạn phải sử dụng một điểm cuối dành riêng cho đối tượng thuê **( https://login.microsoftonline.com/{TenantId_or_Name})** hoặc **điểm cuối của** tổ chức.
    - Tài khoản cá nhân được mời tham gia đối tượng thuê Azure AD không thể sử dụng ROPC.
    - Các tài khoản không có mật khẩu sẽ không thể đăng nhập thông qua ROPC. Đối với kịch bản này, chúng tôi khuyên bạn nên sử dụng một dòng khác cho ứng dụng của mình thay vào đó.
    - Nếu người dùng cần sử dụng [xác thực đa yếu tố (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) để đăng nhập vào ứng dụng, họ sẽ bị chặn.
    - ROPC không được hỗ trợ trong [các kịch](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) bản liên kết định danh kết hợp (ví dụ: Azure AD và ADFS được sử dụng để xác thực tài khoản tại chỗ). Nếu người dùng được chuyển hướng toàn bộ trang đến nhà cung cấp định danh tại chỗ, Azure AD sẽ không thể kiểm tra tên người dùng và mật khẩu đối với nhà cung cấp định danh đó. [Tuy nhiên, xác thực](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) chuyển qua được hỗ trợ với ROPC.
    - Trường hợp liên kết định danh kết hợp sẽ là ngoại lệ như sau: Chính sách Khám phá khu vực trang chủ với **AllowCloudPasswordValidation** được đặt thành **TRUE** sẽ cho phép dòng ROPC hoạt động đối với người dùng được liên kết khi mật khẩu tại chỗ được đồng bộ với đám mây. Để biết thêm thông tin, xem mục [Cho phép xác thực ROPC trực tiếp của người dùng được liên kết cho các ứng dụng thừa tự](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Nền tảng định danh Microsoft và OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) Thay mặt cho dòng - Bài viết này mô tả cách lập trình trực tiếp dựa trên dòng thay mặt **(OBO)** trong ứng dụng của bạn.
- Nền tảng định danh Microsoft và giao thức [Kết nối OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Bài viết này trình bày cách thực thi giao thức Kết nối OpenID độc lập với ngôn ngữ và mô tả cách gửi và nhận thư HTTP mà không sử dụng bất cứ thư viện mã nguồn mở nào của Microsoft.

**Mã thông báo Truy nhập**

[Nền tảng định danh Microsoft thông báo truy nhập mới](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Tìm hiểu cách API của bạn có thể xác thực và sử dụng các khiếu nại bên trong mã thông báo truy nhập. Tất cả tài liệu trong bài viết này, ngoại trừ những trường hợp được ghi chú, chỉ áp dụng cho các mã thông báo được phát hành cho các API bạn đã đăng ký. Thông báo này không áp dụng cho các mã thông báo được phát hành cho các API do Microsoft sở hữu, cũng như không thể sử dụng các mã thông báo đó để xác thực cách Nền tảng định danh Microsoft sẽ phát hành mã thông báo cho một API mà bạn tạo.

**Cấu hình Ứng dụng**

[Giới hạn và giới hạn của URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url) chuyển hướng (URL trả lời) - Tìm hiểu cách đặt cấu hình URI Chuyển hướng (URL trả lời). A redirect URI, or reply URL, is the location where the authorization server sends the user once the app has been successfully authorized and granted an authorization code or access token. Máy chủ ủy quyền gửi mã hoặc mã thông báo đến URI chuyển hướng; vì vậy điều quan trọng là bạn phải đăng ký vị trí chính xác như một phần của quy trình đăng ký ứng dụng.

**Cấp phép Ứng dụng**

[Hướng dẫn: Phát](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) triển và lập kế hoạch cung cấp cho điểm cuối SCIM - Bài viết này mô tả cách xây dựng một điểm cuối SCIM và tích hợp với dịch vụ cung cấp AAD.


