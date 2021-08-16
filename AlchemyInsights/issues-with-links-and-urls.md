---
title: Sự cố với liên kết và URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 1387d7e0cdf2e730b2812f3970181d2bf889d44b1faab9a351911840909defb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054820"
---
# <a name="issues-with-links-and-urls"></a>Sự cố với liên kết và URL

Chuyển hướng URI/URL trả lời (cả hai biểu thức có thể thay đổi) là các URL được sử dụng bởi Nền tảng định danh Microsoft để trả về mã thông báo được yêu cầu ứng dụng. Để biết thông tin về các URL này, hãy xem các bài viết sau đây:

- [Quy trình xác thực và kịch bản ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Thông tin về API chuyển hướng trong trang Đăng **ký** ứng dụng cho từng kịch bản.
- [Giới hạn và giới hạn của URL chuyển hướng URI/trả lời](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Tôi không biết cách đăng ký URI chuyển hướng phù hợp / URL trả lời cho ứng dụng của tôi**

Khi bạn đăng nhập bằng ứng dụng mà bạn đang phát triển, nếu hộp thoại đăng nhập hiển thị **AADSTS50011: URL <your app ID>** trả lời được chỉ định trong yêu cầu không khớp với url trả lời được cấu hình cho ứng dụng , bạn sẽ cần thêm vào đăng ký ứng dụng của mình, URI chuyển hướng mà mã của bạn dùng trong yêu cầu mã thông báo đến Nền tảng định danh Microsoft.

Để thêm URL trả lời, hãy  đi đến **tab** Xác thực trong trang đăng ký ứng dụng của bạn trong cổng thông tin Azure và thêm một mục nhập trong mục **LỐI DẪN Chuyển** hướng. Giá trị bạn cần nhập phụ thuộc vào loại ứng dụng bạn đang tạo, như mô tả dưới đây:

- Đối với các ứng dụng trang đơn và ứng dụng web, URL trả lời là một URL trong ứng dụng của bạn. Xem [Đăng ký ứng dụng một trang hoặc](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) Đăng ký ứng dụng web bằng cổng thông tin [Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Đối với các ứng dụng trên máy tính, giá trị mà bạn cần chọn phụ thuộc vào:
    - nền tảng (MacOS khác với Windows Linux)
    - cách bạn nhận được mã thông báo (tương tác với dòng mã thiết bị, với Xác thực Windows Tích hợp [IWA] hoặc với tên người dùng/mật khẩu).
    Để biết chi tiết, xem mục [Ứng dụng trên máy tính - Đăng ký ứng dụng - Chuyển hướng giao diện người dùng](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Đối với các ứng dụng dành cho thiết bị di động, URI chuyển hướng phụ thuộc vào:
    - nền tảng (iOS/Android/UWP)
    - thông tin được dùng để xây dựng ứng dụng của bạn, chẳng hạn như ID gói trong iOS và tên gói và băm chữ ký trên Android Việc đăng ký ứng dụng cổng thông tin Azure sẽ giúp bạn. Để biết chi tiết, hãy [xem Cấu hình nền tảng và URL chuyển hướng](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Các API web và một số cách im lặng của việc mua mã thông báo (IWA và tên người dùng/mật khẩu) không yêu cầu URI chuyển hướng.

**Tôi đã triển khai ứng dụng web của mình và khi tôi kiểm tra ứng dụng đã triển khai, tôi nhận được thông báo url trả lời không khớp**

Thêm URL chuyển hướng cho tất cả các vị trí mà tại đó bạn đang triển khai ứng dụng web của bạn. Để biết thêm thông tin, hãy [xem Đăng ký ứng dụng web bằng cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Thêm URI chuyển hướng cho vị trí ngay sau khi bạn đã triển khai ứng dụng tại vị trí đó.

**Tôi không thể đăng ký đủ URL trả lời**

Bạn là một ISV và có một hoặc một vài URL chuyển hướng cho mọi khách hàng của bạn. Bạn muốn di chuyển từ ADAL/Azure AD v1.0 sang MSAL/Nền tảng định danh Microsoft và nhấn vào số lượng [URL chuyển hướng tối đa.](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris) Để giải quyết vấn đề này, [hãy thêm các URL chuyển hướng vào tên dịch vụ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) chính tương ứng với từng khách hàng của bạn.
