---
title: Sự cố phát triển ứng dụng với API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013482"
---
# <a name="issues-developing-applications-with-apis"></a>Sự cố phát triển ứng dụng với API

Để bắt đầu sử dụng API Azure Active Directory Graph, hãy xem hướng dẫn nhanh [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) hoặc xem hướng dẫn tham khảo Azure AD Graph API tương [tác.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL) và API Graph Azure AD (AAD Graph)**

**Kể từ ngày 30 tháng 6 năm 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào ADAL và Azure AD Graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.

Bắt đầu **từ ngày 30 tháng 6 năm 2022,** chúng tôi sẽ kết thúc hỗ trợ cho ADAL và Azure AD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa.

Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.

Các ứng dụng sử dụng Azure AD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối Azure AD Graph lại.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật [lên Thư viện Xác thực Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)nơi có các tính năng và bản cập nhật bảo mật mới nhất.

Nếu bạn đang sử dụng các ứng dụng của Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ, nhằm đảm bảo rằng chúng sẽ hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

1. [Đọc Câu hỏi thường gặp về ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Nếu bạn cần trợ giúp để hiểu rõ ứng dụng nào sử dụng ADAL, chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có thể, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.

**Di chuyển thiết Graph AAD**

Đối với các ứng dụng đang sử dụng Azure AD Graph, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng [Azure AD Graph sang Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
1. Cổng thông tin đăng ký ứng dụng Azure của bạn hiển thị các ứng dụng đang sử dụng AAD Graph. Chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các hoạt động sử Graph AAD trong đối tượng thuê của bạn.
1. Để ứng dụng của bạn truy nhập dữ liệu trong Microsoft Graph, người dùng hoặc người quản trị phải cấp đúng quyền thông qua một quy trình đồng ý. Tham [chiếu quyền Graph Microsoft liệt](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) kê các quyền liên kết với mỗi tập hợp chính của Microsoft Graph API. Tài liệu cũng cung cấp hướng dẫn về cách sử dụng các quyền.
