---
title: Khắc phục sự cố Đăng nhập Một lần Đăng nhập Một lần (SSO) dựa trên mật khẩu
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
- "9374"
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972846"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Khắc phục sự cố Đăng nhập Một lần Đăng nhập Một lần (SSO) dựa trên mật khẩu

Để tìm hiểu các nguyên tắc cơ bản của SSO dựa trên mật khẩu, hãy [xem Xác thực dựa trên mật khẩu Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Đặt cấu hình SSO dựa trên Mật khẩu**

1. [Đặt cấu hình đăng nhập đơn dựa trên mật khẩu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - Bài viết này sẽ giải thích chi tiết hơn về tùy chọn SSO dựa trên mật khẩu. Nếu ứng dụng bạn đang thêm yêu cầu cấu hình tùy chỉnh và bạn cần sử dụng SSO dựa trên mật khẩu thì bài viết này là dành cho bạn.
2. [Cấu hình đăng nhập đơn dựa trên mật khẩu đối với các ứng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) dụng tại cơ sở - Proxy Ứng dụng hỗ trợ một số chế độ đăng nhập một lần. Đăng nhập dựa trên mật khẩu dành cho các ứng dụng sử dụng kết hợp tên người dùng/mật khẩu để xác thực. Khi bạn cấu hình đăng nhập dựa trên mật khẩu cho ứng dụng của bạn, người dùng của bạn phải đăng nhập vào ứng dụng tại chỗ một lần. Sau đó, Azure Active Directory lưu trữ thông tin đăng nhập và tự động cung cấp thông tin đó cho ứng dụng khi người dùng của bạn truy nhập từ xa.
    - Lẽ ra bạn đã phát hành và kiểm tra ứng dụng của mình bằng Proxy Ứng dụng. Nếu không, hãy làm theo các bước trong Phát hành ứng dụng bằng [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) sau đó tiếp tục cấu hình SSO dựa trên mật khẩu cho các ứng dụng tại cơ sở.

Để khắc phục sự cố SSO dựa trên mật khẩu, hãy xem mục Khắc phục sự cố đăng [nhập một lần dựa trên mật khẩu trong Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
