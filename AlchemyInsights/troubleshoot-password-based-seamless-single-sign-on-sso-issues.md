---
title: Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) dựa trên mật khẩu
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
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714910"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) dựa trên mật khẩu

Để tìm hiểu các nguyên tắc cơ bản của SSO dựa trên mật khẩu, hãy xem [xác thực dựa trên mật khẩu với Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Đặt cấu hình SSO dựa trên mật khẩu**

1. [Đặt cấu hình đăng nhập đơn dựa trên mật khẩu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -bài viết này đi sâu vào chi tiết hơn về tùy chọn SSO dựa trên mật khẩu. Nếu ứng dụng bạn đang thêm yêu cầu cấu hình tùy chỉnh và bạn cần sử dụng SSO dựa trên mật khẩu, thì bài viết này là dành cho bạn.
2. [Đặt cấu hình đăng nhập đơn dựa trên mật khẩu cho ứng dụng Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -proxy hỗ trợ một số chế độ đăng nhập đơn. Đăng nhập dựa trên mật khẩu được dành cho các ứng dụng sử dụng kết hợp tên người dùng/mật khẩu để xác thực. Khi bạn cấu hình đăng ký dựa trên mật khẩu cho ứng dụng của bạn, người dùng của bạn phải đăng nhập vào ứng dụng tại cơ sở một lần. Sau đó, Azure Active Directory lưu trữ thông tin đăng nhập và tự động cung cấp cho ứng dụng khi người dùng của bạn truy nhập từ xa.
    - Bạn nên đã được phát hành và thử nghiệm ứng dụng của bạn với proxy ứng dụng. Nếu không, hãy làm theo các bước trong phát hành các [ứng dụng bằng cách sử dụng ứng dụng AZURE AD proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) sau đó tiếp tục cấu hình của bạn trong SSO dựa trên mật khẩu cho các ứng dụng trên Prem.

Để khắc phục sự cố SSO dựa trên mật khẩu, hãy xem [khắc phục sự cố đăng nhập đơn trên mật khẩu trong AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
