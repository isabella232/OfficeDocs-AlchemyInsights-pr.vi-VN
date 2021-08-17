---
title: Làm việc với Thư viện Xác thực
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: b667e699e1595b21d80788123de13daffbe79a35b1671e9d35eaa6cd980693db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083108"
---
# <a name="working-with-authentication-libraries"></a>Làm việc với Thư viện Xác thực

Để giải quyết sự cố Thư viện Xác thực Microsoft (MSAL), hãy thực hiện các bước được đề xuất sau đây:

1. **Làm việc với MSAL**: thư [Nền tảng định danh Microsoft xác thực -](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Bài viết này hiển thị hỗ trợ Thư viện Xác thực Microsoft cho một số loại ứng dụng. Mẫu này bao gồm các nối kết đến mã nguồn thư viện; nơi nhận gói hàng cho dự án của ứng dụng; và thư viện đó hỗ trợ đăng nhập người dùng (xác thực), truy nhập vào các API web được bảo vệ (ủy quyền) hay cả hai.

2. **Xác thực Khắc** phục sự cố : MSAL hỗ trợ một số dòng xác thực để sử dụng trong các kịch bản ứng dụng khác nhau. Tùy thuộc vào cách xây dựng ứng dụng máy khách của bạn, MSAL có thể sử dụng một hoặc nhiều dòng xác thực được dòng xác thực mà tổ chức Nền tảng định danh Microsoft. Các dòng này có thể tạo ra một số loại mã thông báo và mã ủy quyền cũng như yêu cầu các mã thông báo khác nhau để chúng hoạt động.

3. **Mã thông báo Truy** nhập : [Nền tảng định danh Microsoft mã thông báo truy](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) nhập - Tìm hiểu cách API của bạn có thể xác thực và sử dụng các khiếu nại bên trong mã thông báo truy nhập. Tất cả tài liệu trong bài viết này, ngoại trừ những trường hợp được ghi chú, chỉ áp dụng cho các mã thông báo được phát hành cho các API bạn đã đăng ký. Thông báo này không áp dụng cho các mã thông báo được phát hành cho các API do Microsoft sở hữu, cũng như không thể sử dụng các mã thông báo đó để xác thực cách Nền tảng định danh Microsoft sẽ phát hành mã thông báo cho một API mà bạn tạo.

**Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL)**

- **Kể từ ngày 30 tháng 6 năm 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào ADAL và Azure AD Graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.
- Bắt đầu **từ ngày 30 tháng 6 năm 2022,** chúng tôi sẽ kết thúc hỗ trợ cho ADAL và Azure AD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa.
- Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ *hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.*
- Các ứng dụng sử dụng Azure AD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối Azure AD Graph lại.

**Di chuyển ADAL**

- Chúng tôi khuyên bạn nên cập nhật lên MSAL, ứng dụng này có các tính năng mới nhất và các bản cập nhật bảo mật.
- Nếu bạn đang sử dụng các ứng dụng của Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ, nhằm đảm bảo rằng chúng sẽ hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

1. [Đọc Câu hỏi thường gặp về ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Nếu sau khi đọc hướng dẫn về nền tảng ứng dụng của bạn, bạn có thêm câu hỏi, bạn có thể đăng lên [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) với thẻ [azure-ad-adal-deprecation] hoặc mở sự cố trong kho lưu trữ GitHub của thư viện. Hãy xem [mục Ngôn ngữ và khuôn khổ](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) của bài viết tổng quan **MSAL** để biết các liên kết đến lần xuất bản của từng thư viện.
4. **Nếu bạn cần trợ giúp để hiểu rõ ứng dụng nào sử dụng ADAL,** chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng. Nếu có thể, hãy liên hệ với bất kỳ nhà cung cấp phần mềm Độc lập (ISV) hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.







