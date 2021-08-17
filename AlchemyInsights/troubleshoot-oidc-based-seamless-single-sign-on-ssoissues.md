---
title: Khắc phục sự cố Đăng nhập Một lần (SSO) dựa trên OIDC
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
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105806"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Khắc phục sự cố Đăng nhập Một lần (SSO) dựa trên OIDC

- Để tìm hiểu cách thêm ứng dụng dựa trên OIDC vào đối tượng thuê Azure của bạn, hãy xem Bắt đầu nhanh: Thiết lập đăng nhập đơn dựa trên [OIDC (SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)cho một ứng dụng trong đối tượng thuê Azure Active Directory (Azure AD) của bạn.
- Để biết thêm chi tiết về các ứng dụng sử dụng tiêu chuẩn Kết nối OpenID để triển khai đăng nhập một lần, xem mục Hiểu rõ đăng nhập đơn dựa [trên OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Để biết thông tin trong trường hợp bạn chọn ghi mã của mình bằng cách gửi và xử lý trực tiếp các yêu cầu HTTP hoặc sử dụng thư viện mã nguồn mở của bên thứ ba, thay vì sử dụng một trong các thư viện mã nguồn mở của chúng tôi, hãy xem các giao thức [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)và OpenID Kết nối trên Nền tảng định danh Microsoft.

**Giao thức**

1. [Nền tảng định danh Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) và ngầm cấp - Đặc tính xác định của khoản cấp ẩn là các mã thông báo (mã thông báo ID hoặc mã thông báo truy nhập) được trả về trực tiếp từ điểm cuối /authorize thay vì điểm cuối /token. Điều này thường được sử dụng như một phần của dòng mã ủy quyền, trong dòng được gọi là "dòng hỗn **hợp" -** truy xuất mã thông báo ID trên yêu cầu /ủy quyền cùng với mã ủy quyền . Bài viết này mô tả cách lập trình trực tiếp đối với giao thức trong ứng dụng của bạn để yêu cầu mã thông báo từ Azure AD.
2. Nền tảng định danh Microsoft và dòng mã ủy quyền [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - có thể sử dụng cấp mã ủy quyền OAuth 2.0 trong các ứng dụng được cài đặt trên thiết bị để có quyền truy nhập vào các tài nguyên được bảo vệ, chẳng hạn như các API web. Sử dụng công Nền tảng định danh Microsoft thực hiện OAuth 2.0, bạn có thể thêm quyền đăng nhập và truy nhập API vào các ứng dụng dành cho thiết bị di động **và máy tính.** Bài viết này mô tả cách lập trình trực tiếp đối với giao thức trong ứng dụng của bạn bằng bất kỳ ngôn ngữ nào.
3. Nền tảng định danh Microsoft giao thức [Kết nối OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - Khi bạn sử dụng việc triển khai OpenID Kết nối Nền tảng định danh Microsoft của Nền tảng định danh Microsoft, bạn có thể thêm quyền đăng nhập và truy nhập API vào các ứng dụng của mình. Bài viết này cho biết cách làm điều này độc lập với ngôn ngữ và mô tả cách gửi và nhận thư HTTP mà không sử dụng bất kỳ **thư viện nguồn mở nào của Microsoft.**
4. Nền tảng định danh Microsoft và dòng thông tin xác thực máy khách [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - Bạn có thể sử dụng thông tin xác thực máy khách OAuth 2.0 được chỉ định trong RFC 6749, đôi khi được gọi là **OAuth** hai chân , để truy nhập các tài nguyên được lưu trữ trên web bằng cách sử dụng danh tính của một ứng dụng. Loại cấp này thường được sử dụng cho các tương tác giữa các máy chủ và máy chủ phải chạy ở nền mà không có tương tác ngay lập tức với người dùng. Những kiểu ứng dụng này thường được gọi là tài **khoản đăng ký hoặc** tài khoản dịch **vụ**. Bài viết này mô tả cách lập trình trực tiếp trên giao thức trong ứng dụng của bạn.
