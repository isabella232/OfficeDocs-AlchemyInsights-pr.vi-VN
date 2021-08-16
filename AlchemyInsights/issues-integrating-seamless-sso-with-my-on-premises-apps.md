---
title: Các sự cố với việc tích hợp Seamless SSO với các ứng dụng tại chỗ của tôi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028314"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Các sự cố với việc tích hợp Seamless SSO với các ứng dụng tại chỗ của tôi

Để khắc phục sự cố với tích hợp Seamless SSO với các ứng dụng tại chỗ, hãy làm như sau:

**Các bước được đề xuất**

1. Để cấu **hình một ứng dụng** tại cơ sở cho đăng nhập đơn qua **Proxy** Ứng dụng , hãy xem Tạo kho mật khẩu để đăng nhập một lần bằng Proxy [Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. Khắc **phục** sự cố Proxy Ứng dụng : chúng tôi khuyên bạn nên bắt đầu với việc xem lại quy trình khắc phục sự cố, Gỡ lỗi Các vấn đề của Trình kết nối Proxy Ứng dụng , để xác định xem bộ nối [Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)Ứng dụng có được cấu hình đúng hay không. Nếu bạn vẫn gặp sự cố kết nối với ứng dụng, hãy làm theo các bước khắc phục sự cố trong [Các vấn đề ứng dụng Proxy Gỡ lỗi Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Bạn có thể [xác định sự cố CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) bằng cách sử dụng các công cụ gỡ lỗi trình duyệt sau đây:
    1. Khởi chạy trình duyệt, rồi duyệt đến ứng dụng web.
    1. Nhấn **F12** để mở bảng điều khiển gỡ lỗi.
    1. Cố gắng tạo lại giao dịch và xem lại thông báo bảng điều khiển. Vi phạm CORS tạo ra lỗi bảng điều khiển về nguồn gốc.
    1. Một số vấn đề CORS không thể được giải quyết, chẳng hạn như khi ứng dụng của bạn chuyển hướng đến login.microsoftonline.com để xác thực và mã thông báo truy nhập hết hạn. Khi đó, không thực hiện được cuộc gọi CORS. Giải pháp thay thế cho kịch bản này là kéo dài thời hạn của mã thông báo truy nhập, để ngăn mã thông báo này hết hạn trong phiên của người dùng. Để biết thêm thông tin về cách làm điều này, hãy xem Thời hạn mã thông báo có thể [cấu hình trong Nền tảng định danh Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Tài liệu được đề xuất**

- [Cách cấu hình đăng nhập đơn vào ứng dụng Proxy Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Đăng nhập đơn SAML cho các ứng dụng tại chỗ với Proxy Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Tìm hiểu và giải Azure Active Directory các vấn đề về CORS Proxy Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Khắc phục sự cố cấu hình ủy quyền bị ràng buộc của Kerberos cho Proxy Ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)