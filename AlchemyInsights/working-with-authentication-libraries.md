---
title: Làm việc với thư viện xác thực
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
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036863"
---
# <a name="working-with-authentication-libraries"></a>Làm việc với thư viện xác thực

Để giải quyết sự cố về thư viện xác thực của Microsoft (MSAL), hãy thực hiện các bước được đề xuất sau đây:

1. **Làm việc với MSAL**: [Thư viện xác thực nền tảng căn cước Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -bài viết này hiển thị hỗ trợ thư viện xác thực Microsoft cho một số loại ứng dụng. Nó bao gồm các nối kết đến mã nguồn thư viện; nơi nhận gói cho dự án ứng dụng của bạn; và liệu thư viện hỗ trợ đăng nhập của người dùng (xác thực), truy nhập vào các API web được bảo vệ (ủy quyền) hoặc cả hai.

2. **Khắc phục sự cố xác thực**: hàm msal hỗ trợ một số dòng xác thực để sử dụng trong các kịch bản ứng dụng khác nhau. Tùy thuộc vào cách thức ứng dụng khách của bạn được xây dựng, thì MSAL có thể sử dụng một hoặc nhiều dòng xác thực được hỗ trợ bởi nền tảng định danh Microsoft. Những dòng này có thể tạo ra một số loại thẻ và mã ủy quyền và yêu cầu các thẻ khác nhau để làm cho chúng hoạt động.

3. **Thẻ Access**: [thẻ truy nhập Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -tìm hiểu cách API của bạn có thể xác thực và sử dụng các tuyên bố bên trong mã thông báo Access. Tất cả tài liệu trong bài viết này, ngoại trừ khi ghi chú, chỉ áp dụng cho các thẻ được phát hành cho các API mà bạn đã đăng ký. Nó không áp dụng cho các thẻ được phát hành cho các API Microsoft thuộc sở hữu, cũng không thể dùng thẻ này để xác thực cách Microsoft Identity Platform sẽ phát hành thẻ cho API bạn tạo ra.

**Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL)**

- **Bắt đầu từ ngày 30 tháng 6, 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Adal và Azure AD graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.
- **Bắt đầu từ ngày 30 tháng 6, 2022,** chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.
- Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không *nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào*.
- Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.

**Di chuyển ADAL**

- Chúng tôi khuyên bạn nên cập nhật lên MSAL, trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.
- Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ bảo mật liên tục và cải thiện tính năng của MSAL.

1. [Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Nếu sau khi đọc hướng dẫn dành cho nền tảng ứng dụng của bạn, bạn có thêm câu hỏi, bạn có thể đăng lên [Microsoft hỏi&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) bằng thẻ [Azure-AD-Adal-deprecation] hoặc mở một vấn đề trong kho lưu trữ của thư viện. Xem phần [ngôn ngữ và khung](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) của bài viết **tổng quan về msal** cho các nối kết đến repo của mỗi thư viện.
4. **Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL**, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn. Nếu áp dụng, hãy tiếp cận với bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.







