---
title: Truy vấn API của Microsoft Graph
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923261"
---
# <a name="querying-the-microsoft-graph-api"></a>Truy vấn API của Microsoft Graph

Chủ đề này cũng có thể áp dụng cho các nhà phát triển vẫn sử dụng Azure AD Graph API. Tuy nhiên, bạn **nên sử dụng** Microsoft Graph tất cả các kịch bản quản lý thư mục, danh tính và truy nhập của mình.

**Các sự cố về xác thực hoặc ủy quyền**

- Nếu ứng  dụng của bạn không thể nhận được mã thông báo để gọi cho Microsoft Graph, hãy chọn Vấn đề với việc nhận một mã thông báo truy nhập **(Xác thực)** Microsoft Graph để nhận được trợ giúp và hỗ trợ cụ thể hơn về chủ đề này.
- Nếu ứng dụng của bạn nhận được lỗi ủy quyền **401 hoặc 403** khi gọi cho Microsoft Graph, hãy chọn danh mục Nhận lỗi truy nhập bị từ chối **(Ủy quyền)** Microsoft Graph API để nhận được trợ giúp và hỗ trợ cụ thể hơn về chủ đề này.

**Tôi muốn sử dụng Microsoft Graph nhưng không chắc nên bắt đầu từ đâu**

Để tìm hiểu thêm về Microsoft Graph, hãy xem:

- [Tổng quan về Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Tổng quan về Quản lý Danh tính và Truy nhập trong Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Bắt đầu xây dựng các ứng dụng Microsoft Graph](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** - Kiểm tra API Microsoft Graph trong đối tượng thuê của bạn hoặc đối tượng thuê demo

**Tôi muốn sử dụng Microsoft Graph, nhưng liệu họ có hỗ trợ API thư mục v1.0 mà tôi cần không?**

Microsoft Graph là API được đề xuất cho quản lý thư mục, danh tính và truy nhập. Tuy nhiên, vẫn có một vài khoảng trống giữa những điều có thể xảy ra trong Azure AD Graph và Microsoft Graph. Xem lại các bài viết sau đây, trong đó nêu bật những khác biệt cập nhật nhất nhằm hỗ trợ bạn lựa chọn:

- [Sự khác biệt về loại tài nguyên giữa Azure AD Graph và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Sự khác biệt về thuộc tính giữa Azure AD Graph và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Sự khác biệt về phương pháp giữa Azure AD và Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Khi tôi truy vấn đối *tượng người dùng,* nhiều thuộc tính của đối tượng bị thiếu**

`GET https://graph.microsoft.com/v1.0/users`chỉ trả về 11 thuộc tính, khi Microsoft Graph động chọn bộ thuộc tính người dùng *mặc* định để trả về. Nếu bạn cần các thuộc *tính người dùng* khác, hãy sử $select để chọn thuộc tính mà ứng dụng của bạn cần. Trước tiên, hãy **dùng thử ứng dụng này trong Microsoft Graph Explorer.**

**Một số giá trị thuộc tính người *dùng là null* ngay cả khi tôi biết chúng được đặt**

Giải thích có khả năng cao nhất là ứng dụng đã được cấp *quyền User.ReadBasic.All.* Điều này cho phép ứng dụng đọc tập hợp giới hạn các thuộc tính người dùng, trả về tất cả các thuộc tính khác dưới dạng null ngay cả khi chúng đã được đặt trước đó. Thay vào đó, hãy thử cấp *quyền User.Read.All* cho ứng dụng.

Để biết thêm thông tin, hãy [xem mục Microsoft Graph quyền người dùng](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Tôi đang gặp sự cố khi sử dụng tham số truy vấn OData để lọc dữ liệu trong yêu cầu của mình**

Mặc dù Microsoft Graph hỗ trợ một phạm vi rộng các tham số truy vấn OData, nhiều tham số trong số đó không được dịch vụ thư mục hỗ trợ đầy đủ (tài nguyên kế thừa từ *directoryObject*) trong Microsoft Graph. Các hạn chế tương tự hiện diện trong Azure AD Graph phần lớn trong Microsoft Graph:

1. **Không hỗ** trợ : $count, $search và các giá $filter có trên *các giá trị null* hoặc *không phải là null*
2. **Không hỗ trợ**: Tùy $filter thuộc tính nhất định (xem chủ đề tài nguyên về những thuộc tính có thể lọc được)
3. **Không được** hỗ trợ : phân trang, lọc và sắp xếp cùng một lúc
4. **Không hỗ trợ**: lọc trên mối quan hệ. Ví dụ - tìm tất cả các thành viên của nhóm kỹ thuật tại Vương quốc Anh.
5. **Hỗ trợ một** phần : hỗ $orderby *trên người* dùng (chỉ displayName và userPrincipalName) và *nhóm*
6. Hỗ trợ một phần **:**$filter (chỉ hỗ trợ *eq*, *startswith* *hoặc* *hoặc* và , và hạn chế hỗ trợ bất kỳ *)*$expand (mở rộng mối quan hệ của một đối tượng duy nhất sẽ trả về tất cả các mối quan hệ nhưng việc mở rộng tập hợp các mối quan hệ của đối tượng bị hạn chế)

Để biết thêm thông tin, xem [mục Tùy chỉnh phản hồi với tham số truy vấn.](https://docs.microsoft.com/graph/query-parameters)

**API tôi đang gọi không hoạt động - tôi có thể thực hiện thêm kiểm tra ở đâu?**

**Microsoft Graph Explorer** - Kiểm tra API Microsoft Graph trong đối tượng thuê của  bạn hoặc đối tượng thuê demo và cũng kiểm tra các truy vấn mẫu trong Microsoft Graph Explorer.

**Khi tôi truy vấn dữ liệu, dường như tôi nhận được thiết lập dữ liệu không đầy đủ**

Nếu bạn đang truy vấn một tuyển tập (chẳng hạn như người *dùng),* Microsoft Graph sẽ sử dụng giới hạn trang phía máy chủ để kết quả luôn được trả về với kích thước trang mặc định. Ứng dụng của bạn sẽ luôn chờ đợi từng trang qua các bộ sưu tập được trả về từ dịch vụ.

Để biết thêm thông tin, hãy xem:

- [Các phương pháp Graph nhất của Microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Phân trang dữ liệu Graph Microsoft trong ứng dụng của bạn](https://docs.microsoft.com/graph/paging)

**Ứng dụng của tôi quá chậm và cũng bị điều tiết. Tôi có thể thực hiện những cải tiến nào?**

Tùy theo kịch bản mà bạn có nhiều tùy chọn khác nhau để ứng dụng của bạn hoạt động hiệu quả hơn và trong một số trường hợp, ít dễ bị điều chỉnh bởi dịch vụ (khi bạn thực hiện quá nhiều cuộc gọi).

Để tìm hiểu thêm, hãy xem:

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
