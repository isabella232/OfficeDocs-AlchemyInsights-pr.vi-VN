---
title: Các vấn đề về kết nối SSO
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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935208"
---
# <a name="sso-connection-issues"></a>Các vấn đề về kết nối SSO

1. Theo dõi [bắt đầu nhanh: cấu hình thuộc tính cho một hướng dẫn ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) để cấu hình ứng dụng của bạn.
2. Tùy thuộc vào tùy chọn ứng dụng và [đăng nhập đơn](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) bạn đã chọn, hãy làm theo hướng dẫn thích hợp dưới đây:
    - Để đặt cấu hình cho một **ứng dụng tại chỗ** cho **đăng nhập đơn dựa trên SAML**, hãy xem mục [đăng nhập một lần cho các ứng dụng tại chỗ với proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Để cấu hình một **ứng dụng đám mây** cho **đăng nhập đơn dựa trên mật khẩu**, hãy xem mục  [đặt cấu hình đăng nhập bằng mật khẩu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Để cấu hình một **ứng dụng tại chỗ** cho **đăng nhập đơn thông qua proxy ứng dụng**, hãy xem [khung vòm mật khẩu cho đăng nhập đơn với proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Khắc phục sự cố về vấn đề proxy ứng dụng**: chúng tôi khuyên bạn nên bắt đầu với việc xem xét dòng khắc phục sự cố, các [vấn đề về trình kết nối proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), để xác định xem bạn có cấu hình đúng không. Nếu bạn vẫn gặp sự cố khi kết nối với ứng dụng, hãy làm theo dòng khắc phục sự cố trong [vấn đề ứng dụng proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Bạn có thể [xác định các vấn đề về CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) bằng cách sử dụng công cụ gỡ lỗi của trình duyệt:
    - Khởi động trình duyệt và duyệt đến ứng dụng web.
    - Nhấn **F12** để đưa lên bàn điều khiển Debug.
    - Tìm cách tái tạo giao dịch và xem lại thông điệp bàn điều khiển. Vi phạm CORS tạo ra lỗi bàn điều khiển về nguồn gốc.
    - Một số không thể giải quyết được sự cố, chẳng hạn như khi ứng dụng của bạn chuyển hướng đến login.microsoft.com để xác thực và mã thông báo Access hết hạn. Sau đó, cuộc gọi CORS không thành công. Một giải pháp thay thế cho kịch bản này là mở rộng thời gian của mã thông báo Access, để tránh không bị hết hạn trong suốt phiên của người dùng. Để biết thêm thông tin về cách thực hiện thao tác này, hãy xem [cấu hình hạn trong Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Khắc phục sự cố đăng nhập đơn dựa trên SAML**: chúng tôi khuyên bạn nên kiểm tra sự [cố khi đăng nhập vào các ứng dụng được đặt cấu hình đăng nhập đơn vào SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), để tìm giải pháp cho các vấn đề bạn có thể gặp phải.
5. **Khắc phục sự cố đăng nhập đơn dựa trên mật khẩu**: chúng tôi khuyên bạn nên kiểm tra việc [khắc phục sự cố đăng nhập đơn dựa trên mật khẩu trong Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), để tìm giải pháp cho các vấn đề mà bạn có thể gặp phải.
6. Đối với các vấn đề về kết nối trong khi sử dụng VPN, hãy xem [cách sử dụng đăng nhập đơn (SSO) qua VPN và các kết nối Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
