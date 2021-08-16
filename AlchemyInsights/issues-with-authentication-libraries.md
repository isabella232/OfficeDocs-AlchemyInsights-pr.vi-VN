---
title: Sự cố với Thư viện Xác thực
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028026"
---
# <a name="issues-with-authentication-libraries"></a>Sự cố với Thư viện Xác thực

1. [Nền tảng định danh Microsoft sẽ liệt kê các](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) thư viện máy khách và phần mềm trung gian tương thích và được Microsoft hỗ trợ.
2. Thư viện Xác thực Của Microsoft (MSAL) hỗ trợ một số [dòng xác thực để sử](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) dụng trong các kịch bản ứng dụng khác nhau.
3. Để xác thực và nhận các mã thông báo, bạn hãy khởi tạo một ứng dụng khách công khai hoặc bí mật mới trong mã của mình. Bạn có thể đặt một số tùy chọn cấu hình khi khởi tạo ứng dụng máy khách trong Thư viện Xác thực của Microsoft (MSAL). Để tìm hiểu thêm, hãy xem tùy [chọn Cấu hình ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL) và API Graph Azure AD (AAD Graph)**

**Kể từ ngày 30 tháng 6 năm 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào ADAL và Azure AD Graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.

Bắt đầu **từ ngày 30 tháng 6 năm 2022,** chúng tôi sẽ kết thúc hỗ trợ cho ADAL và Azure AD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa.

Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ *hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.*

Các ứng dụng sử dụng Azure AD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối Azure AD Graph lại.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật [lên Thư viện Xác thực Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)nơi có các tính năng và bản cập nhật bảo mật mới nhất.

Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ, để đảm bảo rằng chúng sẽ được hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

Để biết thêm thông tin, hãy xem:

1. [Đọc Câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Nếu bạn cần trợ giúp để hiểu rõ ứng dụng nào sử dụng ADAL, chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có thể, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.

**Di chuyển thiết Graph AAD**

Đối với các ứng dụng đang sử dụng Azure AD Graph, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng [Azure AD Graph sang Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Cổng thông tin đăng ký ứng dụng Azure của bạn hiển thị các ứng dụng đang sử dụng AAD Graph. Chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các hoạt động sử Graph AAD trong đối tượng thuê của bạn.
3. Để ứng dụng của bạn truy nhập dữ liệu trong Microsoft Graph, người dùng hoặc người quản trị phải cấp đúng quyền thông qua một quy trình đồng ý. Tham [chiếu quyền Graph Microsoft liệt](https://docs.microsoft.com/graph/permissions-reference) kê các quyền liên kết với mỗi tập hợp chính của Microsoft Graph API. Tài liệu cũng cung cấp hướng dẫn về cách sử dụng các quyền.
