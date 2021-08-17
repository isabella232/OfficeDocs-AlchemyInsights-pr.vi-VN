---
title: Sự cố kết nối SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084368"
---
# <a name="sso-connection-issues"></a>Sự cố kết nối SSO

1. Thực hiện theo Hướng [dẫn nhanh: Cấu hình thuộc tính cho hướng dẫn ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) để cấu hình ứng dụng của bạn.
2. Tùy thuộc vào ứng dụng và [tùy chọn Đăng nhập một lần mà bạn](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) đã chọn, hãy làm theo hướng dẫn thích hợp dưới đây:
    - Để cấu **hình** một ứng dụng tại cơ sở cho đăng nhập đơn dựa trên **SAML,** hãy xem mục Đăng nhập đơn [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)cho các ứng dụng tại chỗ bằng Proxy Ứng dụng .
    - Để cấu hình **ứng dụng đám mây** cho đăng nhập đơn dựa trên mật **khẩu, hãy** xem [Cấu hình đăng nhập một lần bằng mật khẩu.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Để cấu **hình một ứng dụng** tại cơ sở cho đăng nhập đơn qua **Proxy** Ứng dụng , hãy xem Tạo kho mật khẩu để đăng nhập một lần bằng Proxy [Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Khắc phục** sự cố Các vấn đề về Proxy Ứng dụng : chúng tôi khuyên bạn nên bắt đầu với việc xem lại dòng khắc phục sự cố, Gỡ lỗi Các vấn đề của Trình kết nối Proxy Ứng dụng , để xác định xem liệu Bộ nối [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Ứng dụng đã được cấu hình đúng hay chưa. Nếu bạn vẫn gặp sự cố khi kết nối với ứng dụng, hãy làm theo quy trình khắc phục sự cố [trong các vấn đề ứng dụng Proxy Gỡ lỗi Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Bạn có thể [xác định sự cố CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) bằng cách sử dụng công cụ gỡ lỗi trình duyệt:
    - Khởi chạy trình duyệt, rồi duyệt đến ứng dụng web.
    - Nhấn **F12** để mở bảng điều khiển gỡ lỗi.
    - Cố gắng tạo lại giao dịch và xem lại thông báo bảng điều khiển. Vi phạm CORS tạo ra lỗi bảng điều khiển về nguồn gốc.
    - Một số vấn đề CORS không thể được giải quyết, chẳng hạn như khi ứng dụng của bạn chuyển hướng đến login.microsoft.com để xác thực và mã thông báo truy nhập hết hạn. Khi đó, không thực hiện được cuộc gọi CORS. Giải pháp thay thế cho kịch bản này là kéo dài thời hạn của mã thông báo truy nhập, để ngăn mã thông báo này hết hạn trong phiên của người dùng. Để biết thêm thông tin về cách làm điều này, hãy xem Thời hạn mã thông báo có thể [cấu hình trong Nền tảng định danh Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. **Khắc phục sự** cố đăng nhập một lần dựa trên SAML : chúng tôi khuyên bạn nên kiểm tra Sự cố khi đăng nhập vào ứng dụng được đặt cấu hình đăng nhập một lần dựa trên [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)để tìm giải pháp cho những sự cố mà bạn dễ gặp phải nhất.
5. **Khắc phục sự** cố đăng nhập một lần dựa trên mật khẩu : chúng tôi khuyên bạn nên kiểm tra Khắc phục sự cố đăng nhập một lần dựa trên mật khẩu trong [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), để tìm ra giải pháp cho những vấn đề bạn dễ gặp nhất.
6. Đối với các sự cố kết nối khi sử dụng VPN, hãy xem Cách sử dụng đăng nhập [đơn (SSO) qua VPN và kết nối Wi-Fi VPN.](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)
