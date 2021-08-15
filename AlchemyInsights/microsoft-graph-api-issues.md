---
title: Sự cố API của Microsoft Graph
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975915"
---
# <a name="microsoft-graph-api-issues"></a>Sự cố API của Microsoft Graph

Chủ đề này cũng có thể áp dụng cho các nhà phát triển vẫn sử dụng Azure AD Graph API. Tuy nhiên, bạn **nên sử dụng** Microsoft Graph tất cả các kịch bản quản lý thư mục, danh tính và truy nhập của mình.

**Các sự cố về xác thực hoặc ủy quyền**

- Nếu ứng  dụng của bạn không thể nhận được mã thông báo để gọi cho Microsoft Graph, hãy chọn Vấn đề với việc nhận một mã thông báo truy nhập **(Xác thực)** Microsoft Graph để nhận được trợ giúp và hỗ trợ cụ thể hơn về chủ đề này.
- Nếu ứng dụng của bạn nhận được lỗi ủy quyền **401 hoặc 403** khi gọi cho Microsoft Graph, hãy chọn danh mục Nhận lỗi truy nhập bị từ chối **(Ủy quyền)** Microsoft Graph API để nhận được trợ giúp và hỗ trợ cụ thể hơn về chủ đề này.

**Tôi muốn sử dụng Microsoft Graph nhưng không chắc nên bắt đầu từ đâu**

- [Tổng quan về Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Tổng quan về Quản lý Danh tính và Truy nhập trong Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Bắt đầu xây dựng các ứng dụng Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Kiểm tra API Microsoft Graph trong đối tượng thuê của bạn hoặc đối tượng thuê demo

**Tôi muốn sử dụng Microsoft Graph, nhưng liệu họ có hỗ trợ API thư mục v1.0 mà tôi cần không?**

Microsoft Graph là API được đề xuất cho quản lý thư mục, danh tính và truy nhập. Tuy nhiên, vẫn có một vài khoảng trống giữa những điều có thể xảy ra trong Azure AD Graph và Microsoft Graph. Xem lại các bài viết sau đây, trong đó nêu bật những khác biệt cập nhật nhất nhằm hỗ trợ bạn lựa chọn:

- [Sự khác biệt về loại tài nguyên giữa Azure AD Graph và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Sự khác biệt về thuộc tính giữa Azure AD Graph và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Sự khác biệt về phương pháp giữa Azure AD và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API mà tôi đang gọi không hoạt động - tôi có thể thực hiện thêm kiểm tra ở đâu?**

**Microsoft Graph Explorer** - Kiểm tra API Microsoft Graph trong đối tượng thuê của  bạn hoặc đối tượng thuê demo và cũng kiểm tra các truy vấn mẫu trong Microsoft Graph Explorer.

**Ứng dụng của tôi quá chậm và cũng bị điều tiết. Tôi có thể thực hiện những cải tiến nào?**

Tùy thuộc vào kịch bản của bạn, có nhiều tùy chọn sẵn có để làm cho ứng dụng của bạn hoạt động hiệu quả hơn và trong một số trường hợp, ít dễ bị điều chỉnh dịch vụ (khi bạn thực hiện quá nhiều cuộc gọi).

- [Các phương pháp Graph nhất của Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Yêu cầu lô](https://docs.microsoft.com/graph/json-batching)
- [Theo dõi thay đổi thông qua truy vấn delta](https://docs.microsoft.com/graph/delta-query-overview)
- [Nhận thông báo về các thay đổi thông qua webhooks](https://docs.microsoft.com/graph/webhooks)
- [Hướng dẫn điều chỉnh](https://docs.microsoft.com/graph/throttling)

**Tôi có thể tìm thêm thông tin về lỗi và sự cố đã biết ở đâu?**

- [Thông tin phản Graph Microsoft](https://docs.microsoft.com/graph/errors)
- [Các sự cố đã biết với Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Tôi có thể kiểm tra trạng thái sẵn sàng của dịch vụ và khả năng kết nối ở đâu?**

Tính khả dụng của dịch vụ và khả năng kết nối của các dịch vụ cơ sở có thể được truy nhập thông qua Microsoft Graph có thể ảnh hưởng đến tính sẵn sàng và hiệu suất tổng thể của Microsoft Graph.

- Để biết Azure Active Directory trạng thái dịch vụ, hãy kiểm tra trạng thái của các dịch **vụ Bảo mật + Căn** cước được liệt kê trong trang trạng thái [Azure.](https://azure.microsoft.com/status/)
- Đối với Office các dịch vụ đóng góp vào Microsoft Graph, hãy kiểm tra trạng thái các dịch vụ được liệt kê trong Bảng điều [Office Trạng thái Dịch vụ](https://portal.office.com/adminportal/home#/servicehealth).

Các Graph về ủy quyền của Microsoft có thể là do một số sự cố khác nhau, đa số là nguyên nhân gây ra lỗi 401 hoặc 403. Ví dụ: tất cả những điều sau đây đều có thể dẫn đến lỗi ủy quyền:

- Quy trình [thu thập mã thông báo truy nhập không chính xác](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Phạm vi quyền được đặt [cấu hình kém](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Thiếu sự chấp [thuận](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL) và API Graph Azure AD (AAD Graph)***

**Kể từ ngày 30 tháng 6 năm 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào ADAL và Azure AD Graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.

Bắt đầu **từ ngày 30 tháng 6 năm 2022,** chúng tôi sẽ kết thúc hỗ trợ cho ADAL và Azure AD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa.

Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ *hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.*

Các ứng dụng sử dụng Azure AD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối Azure AD Graph lại.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật [lên Thư viện Xác thực Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)nơi có các tính năng và bản cập nhật bảo mật mới nhất.

Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ, để đảm bảo rằng chúng sẽ hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

1. [Đọc Câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Nếu bạn cần trợ giúp để hiểu rõ ứng dụng nào sử dụng ADAL, chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có thể, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.

**Di chuyển thiết Graph AAD**

Đối với các ứng dụng đang sử dụng Azure AD Graph, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng [Azure AD Graph sang Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Cổng thông tin đăng ký ứng dụng Azure của bạn hiển thị các ứng dụng đang sử dụng AAD Graph. Chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các hoạt động sử Graph AAD trong đối tượng thuê của bạn.
3. Để ứng dụng của bạn truy nhập dữ liệu trong Microsoft Graph, người dùng hoặc người quản trị phải cấp đúng quyền thông qua một quy trình đồng ý. Tham [chiếu quyền Graph Microsoft liệt](https://docs.microsoft.com/graph/permissions-reference) kê các quyền liên kết với mỗi tập hợp chính của Microsoft Graph API. Tài liệu cũng cung cấp hướng dẫn về cách sử dụng các quyền.
