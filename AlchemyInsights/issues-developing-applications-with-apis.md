---
title: Các vấn đề đang phát triển các ứng dụng với API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975023"
---
# <a name="issues-developing-applications-with-apis"></a>Các vấn đề đang phát triển các ứng dụng với API

Để bắt đầu sử dụng API của Azure Active Directory graph, hãy xem [hướng dẫn bắt đầu của AZURE AD graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , hoặc xem [tài liệu tham khảo của AZURE AD graph API tương tác](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and Azure AD graph API (đồ họa Bad)**

**Bắt đầu từ ngày 30 tháng 6, 2020**, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Adal và Azure AD graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.

**Bắt đầu từ ngày 30 tháng 6, 2022**, chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.

Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào.

Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật lên [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.

Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ bảo mật liên tục và cải thiện tính năng của MSAL.

1. [Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.

**Di chuyển đồ thị trong Bad**

Đối với các ứng dụng đang sử dụng đồ thị Azure AD, hãy làm theo hướng dẫn của chúng tôi để di chuyển các [ứng dụng đồ thị AZURE AD sang Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad. Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả việc sử dụng đồ thị trong đối tượng thuê của bạn.
1. Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận. [Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph. Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.
