---
title: Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) trên nền tảng OIDC
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747136"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) trên nền tảng OIDC

- Để tìm hiểu cách thêm ứng dụng dựa trên OIDC vào đối tượng Azure của bạn, hãy xem [bắt đầu nhanh: thiết lập đăng nhập vào OIDC (SSO) cho một ứng dụng trong đối tượng thuê Azure Active Directory (AZURE AD) của bạn](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Để biết thêm chi tiết về các ứng dụng sử dụng tiêu chuẩn kết nối OpenID để thực hiện đăng nhập đơn, hãy xem mục [Tìm hiểu đăng nhập OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Để biết thông tin trong trường hợp bạn chọn để viết mã của bạn bằng cách gửi trực tiếp và xử lý các yêu cầu HTTP hoặc sử dụng thư viện nguồn mở của bên thứ ba, thay vì sử dụng một trong các thư viện nguồn mở của chúng tôi, hãy xem mục [OAuth 2,0 và OpenID kết nối giao thức trên nền tảng định danh Microsoft](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Å**

1. [Nền tảng Microsoft Identity và dòng cấp tiềm ẩn](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) -các đặc tính xác định của Grant tiềm ẩn là thẻ (thẻ ID hoặc thẻ truy nhập) được trả về trực tiếp từ điểm cuối/ủy nhiệm thay vì điểm cuối/token. Điều này thường được sử dụng như một phần của dòng mã ủy quyền, trong điều gì được gọi là **"dòng hỗn hợp"-truy xuất mã thông báo ID theo yêu cầu/ủy quyền cùng với một mã ủy quyền**. Bài viết này mô tả cách chương trình trực tiếp chống lại giao thức trong ứng dụng của bạn để yêu cầu thẻ từ Azure AD.
2. [Nền tảng Microsoft Identity và dòng mã ủy quyền oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) -cấp phép mã oauth 2,0 có thể được sử dụng trong các ứng dụng được cài đặt trên một thiết bị để truy nhập vào các tài nguyên được bảo vệ, chẳng hạn như các API web. Sử dụng Microsoft Identity Platform thực hiện của OAuth 2,0, bạn có thể **Thêm đăng nhập và truy nhập API vào ứng dụng di động và máy tính bàn của bạn**. Bài viết này mô tả cách chương trình trực tiếp chống lại giao thức trong ứng dụng của bạn bằng bất kỳ ngôn ngữ nào.
3. [Microsoft Identity Platform và giao thức kết nối OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) -khi bạn sử dụng triển khai kết nối OpenID Identity Platform của Microsoft, bạn có thể thêm đăng nhập và truy nhập API vào ứng dụng của mình. Bài viết này trình bày cách làm điều này độc lập với ngôn ngữ và mô tả cách **gửi và nhận thư http mà không cần sử dụng bất kỳ thư viện nguồn mở nào của Microsoft**.
4. [Nền tảng Microsoft Identity và dòng chứng danh máy khách oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -bạn có thể dùng cấp chứng danh máy khách oauth 2,0 đã xác định trong RFC 6749, đôi khi được gọi là **hai chân OAuth**, để truy nhập vào các tài nguyên được lưu trữ trên web bằng cách sử dụng danh tính của một ứng dụng. Loại tài trợ này thường được sử dụng cho các tương tác máy chủ phải chạy trong nền, không có sự tương tác ngay lập tức với người dùng. Những loại ứng dụng này thường được gọi là tài khoản **daemons** hoặc **dịch vụ**. Bài viết này mô tả cách chương trình trực tiếp chống lại giao thức trong ứng dụng của bạn.
