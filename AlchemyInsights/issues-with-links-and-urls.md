---
title: Các vấn đề với liên kết và URL
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
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707904"
---
# <a name="issues-with-links-and-urls"></a>Các vấn đề với liên kết và URL

URL chuyển hướng/trả lời (cả hai biểu thức đều có thể hoán đổi) là các URL được dùng bởi nền tảng định danh Microsoft để trả về các thẻ yêu cầu ứng dụng. Để biết thông tin về các URL này, hãy xem các bài viết sau đây:

- Các [dòng xác thực và kịch bản ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -thông tin về việc chuyển hướng đến URIs trong trang **đăng ký ứng dụng** cho từng tình huống.
- [Các hạn chế và giới hạn URL chuyển hướng URI/trả lời](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Tôi không biết làm thế nào để đăng ký URI chuyển hướng bên phải/trả lời URL cho ứng dụng của tôi**

Khi bạn đăng nhập bằng ứng dụng bạn đang phát triển, nếu hộp thoại đăng nhập Hiển thị **AADSTS50011: URL trả lời được xác định trong yêu cầu không khớp với URL trả lời được <your app ID> cấu hình cho ứng dụng**, bạn sẽ cần phải thêm vào đăng ký ứng dụng của mình, URI chuyển hướng mà mã của bạn được sử dụng trong yêu cầu mã thông báo đến nền tảng Microsoft Identity.

Để thêm URL trả lời, hãy đi đến tab **xác thực** trong trang **đăng ký ứng dụng** của bạn trong cổng thông tin Azure và thêm một mục nhập trong phần **chuyển hướng URIs** . Giá trị bạn cần nhập tùy thuộc vào loại ứng dụng mà bạn đang xây dựng, như được mô tả dưới đây:

- Đối với các ứng dụng trang đơn và ứng dụng web, URL trả lời là một URL trong ứng dụng của bạn. Xem [đăng ký ứng dụng trang đơn](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) hoặc [đăng ký ứng dụng Web App bằng cách dùng Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Đối với các ứng dụng trên máy tính, giá trị mà bạn cần chọn tùy thuộc vào:
    - nền tảng (MacOS khác với Windows hoặc Linux)
    - cách bạn thu thập mã thông báo (tương tác, với dòng mã thiết bị, với xác thực Windows tích hợp [IWA] hoặc với tên người dùng/mật khẩu).
    Để biết chi tiết, hãy xem [ứng dụng trên máy tính-đăng ký ứng dụng-URi chuyển hướng](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Đối với các ứng dụng dành cho thiết bị di động, URI chuyển hướng phụ thuộc vào:
    - nền tảng (iOS/Android/UWP)
    - thông tin được sử dụng để xây dựng ứng dụng của bạn, chẳng hạn như ID gói trong iOS và tên gói và chữ ký băm trên thiết bị đăng ký ứng dụng Azure Portal sẽ giúp bạn. Để biết chi tiết, hãy xem [cấu hình nền tảng và chuyển hướng URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Các API web và một số cách thức để có được thẻ (IWA và tên người dùng/mật khẩu) không yêu cầu một URI chuyển hướng.

**Tôi đã triển khai ứng dụng web của mình và khi tôi kiểm tra ứng dụng đã triển khai, tôi nhận được thông báo không khớp với URL trả lời**

Thêm chuyển hướng URIs cho tất cả các vị trí mà tại đó bạn đang triển khai ứng dụng web của bạn. Để biết thêm thông tin, hãy xem mục [đăng ký ứng dụng Web App bằng Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Thêm URI chuyển hướng cho một vị trí ngay sau khi bạn đã triển khai ứng dụng tại vị trí đó.

**Tôi không thể đăng ký đủ URL trả lời**

Bạn là một ISV và có một hoặc nhiều chuyển hướng URIs cho mọi khách hàng của bạn. Bạn muốn di chuyển từ ADAL/Azure AD v 1.0 sang MSAL/nền tảng định danh Microsoft và bạn nhấn vào [số lượng chuyển hướng tối đa của URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Để giải quyết vấn đề này, hãy [Thêm chuyển hướng URIs vào hiệu trưởng dịch vụ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) tương ứng với từng khách hàng của bạn.
