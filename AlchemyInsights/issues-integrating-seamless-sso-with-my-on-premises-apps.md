---
title: Các vấn đề với việc tích hợp SSO liền mạch với các ứng dụng tại chỗ của tôi
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868772"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Các vấn đề với việc tích hợp SSO liền mạch với các ứng dụng tại chỗ của tôi

Để khắc phục sự cố với việc tích hợp SSO liền mạch với các ứng dụng tại cơ sở, hãy làm như sau:

**Các bước được đề xuất**

1. Để cấu hình một **ứng dụng tại chỗ** cho **đăng nhập đơn thông qua proxy ứng dụng**, hãy xem [khung vòm mật khẩu cho đăng nhập đơn với proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Khắc phục sự cố về vấn đề proxy ứng dụng**: chúng tôi khuyên bạn nên bắt đầu với việc xem xét dòng khắc phục sự cố, các [vấn đề về trình kết nối proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), để xác định xem bạn có cấu hình đúng không. Nếu bạn vẫn gặp sự cố khi kết nối với ứng dụng, hãy làm theo các bước khắc phục sự cố trong các [vấn đề về ứng dụng proxy ứng dụng gỡ lỗi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Bạn có thể [xác định các vấn đề về CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) bằng cách sử dụng các công cụ gỡ lỗi của trình duyệt sau:
    1. Khởi động trình duyệt và duyệt đến ứng dụng web.
    1. Nhấn **F12** để đưa lên bàn điều khiển Debug.
    1. Tìm cách tái tạo giao dịch và xem lại thông điệp bàn điều khiển. Vi phạm CORS tạo ra lỗi bàn điều khiển về nguồn gốc.
    1. Một số không thể giải quyết được sự cố, chẳng hạn như khi ứng dụng của bạn chuyển hướng đến login.microsoftonline.com để xác thực và mã thông báo Access hết hạn. Sau đó, cuộc gọi CORS không thành công. Một giải pháp thay thế cho kịch bản này là mở rộng thời gian của mã thông báo Access, để tránh không bị hết hạn trong suốt phiên của người dùng. Để biết thêm thông tin về cách thực hiện thao tác này, hãy xem [cấu hình hạn trong Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Tài liệu được đề xuất**

- [Cách đặt cấu hình đăng nhập một lần vào ứng dụng proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Đăng nhập đơn SAML cho các ứng dụng tại chỗ với proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Tìm hiểu và giải quyết các vấn đề về dữ liệu proxy của ứng dụng Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Khắc phục các cấu hình ủy quyền của Kerberos ràng buộc cho proxy ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)