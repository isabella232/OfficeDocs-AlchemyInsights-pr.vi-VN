---
title: Các vấn đề về API của Microsoft graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714519"
---
# <a name="microsoft-graph-api-issues"></a>Các vấn đề về API của Microsoft graph

Chủ đề này cũng có thể áp dụng cho các nhà phát triển vẫn sử dụng API đồ thị Azure AD. Tuy nhiên, chúng **tôi khuyên bạn nên sử** dụng Microsoft graph cho tất cả các kịch bản, danh tính và tình huống quản lý truy nhập của bạn.

**Các vấn đề về xác thực hoặc ủy quyền**

- Nếu ứng dụng của bạn **không thể** có được thẻ để gọi tới Microsoft graph, hãy chọn **vấn đề với thể loại mã thông báo Access (xác thực)** Microsoft graph để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.
- Nếu ứng dụng của bạn nhận được các **lỗi ủy quyền 401 hoặc 403** khi gọi cho Microsoft graph, hãy chọn thể loại **nhận được một lỗi truy nhập bị từ chối (ủy quyền)** Microsoft graph API để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.

**Tôi muốn sử dụng Microsoft graph, nhưng không chắc chắn bắt đầu từ đâu**

- [Tổng quan về Microsoft graph](https://docs.microsoft.com/graph/overview)
- [Tổng quan về danh tính và quản lý Access trong Microsoft graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Bước bắt đầu xây dựng ứng dụng Microsoft graph](https://docs.microsoft.com/graph/)
- **Microsoft graph Explorer** -kiểm tra API của Microsoft graph trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu

**Tôi muốn sử dụng Microsoft graph nhưng nó hỗ trợ các API của v 1,0 Directory tôi cần?**

Microsoft graph là API được đề xuất cho thư mục, danh tính và quản lý Access. Tuy nhiên, vẫn có một vài khoảng trống giữa những gì có thể có trong Azure AD graph và Microsoft graph. Xem lại các bài viết sau đây, trong đó sẽ tô sáng các điểm khác biệt Cập Nhật nhất để hỗ trợ trong lựa chọn của bạn:

- [Sự khác biệt về kiểu tài nguyên giữa Azure AD graph và Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Sự khác biệt về tài sản giữa Azure AD graph và Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Sự khác biệt về phương pháp giữa Azure AD và đồ thị Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API tôi đang gọi không hoạt động-tôi có thể làm việc kiểm tra khác ở đâu?**

**Microsoft graph Explorer** -kiểm tra API đồ thị Microsoft trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu và cũng có thể xem các **truy vấn mẫu** trong Microsoft graph Explorer.

**Ứng dụng của tôi quá chậm và cũng đang nhận được Throttled. Tôi có thể thực hiện những cải thiện nào?**

Tùy thuộc vào tình huống của bạn, có nhiều tùy chọn khác nhau trong việc xử lý của bạn để làm cho ứng dụng của bạn thêm performant, và trong một số trường hợp, ít dễ bị Throttled bởi dịch vụ (khi bạn đang thực hiện quá nhiều cuộc gọi).

- [Các biện pháp tốt nhất của Microsoft graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Các yêu cầu về định lượng](https://docs.microsoft.com/graph/json-batching)
- [Theo dõi thay đổi thông qua truy vấn đồng bằng](https://docs.microsoft.com/graph/delta-query-overview)
- [Nhận thông báo về các thay đổi thông qua webhooks](https://docs.microsoft.com/graph/webhooks)
- [Hướng dẫn throttling](https://docs.microsoft.com/graph/throttling)

**Tôi có thể tìm thêm thông tin về các lỗi và các vấn đề đã biết ở đâu?**

- [Thông tin phản hồi về lỗi của Microsoft graph](https://docs.microsoft.com/graph/errors)
- [Các vấn đề đã biết với Microsoft graph](https://docs.microsoft.com/graph/known-issues)

**Tôi có thể kiểm tra trạng thái sẵn dùng và khả năng kết nối của dịch vụ ở đâu?**

Tính khả dụng của dịch vụ và kết nối của các dịch vụ cơ bản có thể được truy nhập thông qua Microsoft graph có thể ảnh hưởng đến tính khả dụng tổng thể và hiệu suất của Microsoft graph.

- Đối với dịch vụ Azure Active Directory Health, hãy kiểm tra trạng thái của dịch vụ **danh tính + bảo mật** được liệt kê trong [trang trạng thái Azure](https://azure.microsoft.com/status/).
- Đối với các dịch vụ Office đóng góp vào Microsoft graph, hãy kiểm tra trạng thái các dịch vụ được liệt kê trong bảng điều khiển trạng thái [dịch vụ Office](https://portal.office.com/adminportal/home#/servicehealth).

Lỗi ủy quyền của Microsoft graph có thể là kết quả của một số vấn đề khác nhau, phần lớn trong số đó tạo ra lỗi 401 hoặc 403. Ví dụ, các thao tác sau có thể dẫn đến lỗi ủy quyền:

- [Dòng mua lại mã](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) thông báo không chính xác
- Phạm vi [quyền](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) được đặt cấu hình kém
- Thiếu sự [đồng ý](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and AZURE AD GRAPH API (đồ họa Bad)_* _

_ * Bắt đầu từ ngày 30 tháng 6, 2020 * *, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào ADAL và Azure AD graph. Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.

**Bắt đầu từ ngày 30 tháng 6, 2022**, chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.

Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không *nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào*.

Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật lên [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.

Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ các cải thiện về bảo mật và tính năng của MSAL.

1. [Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.

**Di chuyển đồ thị trong Bad**

Đối với các ứng dụng đang sử dụng đồ thị Azure AD, hãy làm theo hướng dẫn của chúng tôi để [di chuyển các ứng dụng đồ thị AZURE AD sang Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad. Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả việc sử dụng đồ thị trong đối tượng thuê của bạn.
3. Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận. [Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph. Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.
