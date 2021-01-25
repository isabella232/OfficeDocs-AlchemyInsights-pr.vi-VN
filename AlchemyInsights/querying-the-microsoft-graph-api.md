---
title: Truy vấn API của Microsoft graph
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974691"
---
# <a name="querying-the-microsoft-graph-api"></a>Truy vấn API của Microsoft graph

Chủ đề này cũng có thể áp dụng cho các nhà phát triển vẫn sử dụng API đồ thị Azure AD. Tuy nhiên, chúng **tôi khuyên bạn nên sử** dụng Microsoft graph cho tất cả các kịch bản, danh tính và tình huống quản lý truy nhập của bạn.

**Các vấn đề về xác thực hoặc ủy quyền**

- Nếu ứng dụng của bạn **không thể** có được thẻ để gọi tới Microsoft graph, hãy chọn **vấn đề với thể loại mã thông báo Access (xác thực)** Microsoft graph để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.
- Nếu ứng dụng của bạn nhận được các **lỗi ủy quyền 401 hoặc 403** khi gọi cho Microsoft graph, hãy chọn thể loại **nhận được một lỗi truy nhập bị từ chối (ủy quyền)** Microsoft graph API để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.

**Tôi muốn sử dụng Microsoft graph, nhưng không chắc chắn bắt đầu từ đâu**

Để tìm hiểu thêm về Microsoft graph, hãy xem:

- [Tổng quan về Microsoft graph](https://docs.microsoft.com/graph/overview)
- [Tổng quan về danh tính và quản lý Access trong Microsoft graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Bước bắt đầu xây dựng ứng dụng Microsoft graph](https://docs.microsoft.com/graph/)
- **Microsoft graph Explorer** -kiểm tra API của Microsoft graph trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu

**Tôi muốn sử dụng Microsoft graph nhưng nó hỗ trợ các API của v 1,0 Directory tôi cần?**

Microsoft graph là API được đề xuất cho thư mục, danh tính và quản lý Access. Tuy nhiên, vẫn có một vài khoảng trống giữa những gì có thể có trong Azure AD graph và Microsoft graph. Xem lại các bài viết sau đây, trong đó sẽ tô sáng các điểm khác biệt Cập Nhật nhất để hỗ trợ trong lựa chọn của bạn:

- [Sự khác biệt về kiểu tài nguyên giữa Azure AD graph và Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Sự khác biệt về tài sản giữa Azure AD graph và Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Sự khác biệt về phương pháp giữa Azure AD và đồ thị Microsoft](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Khi tôi truy vấn đối tượng *người dùng* , nhiều thuộc tính của nó bị thiếu**

`GET https://graph.microsoft.com/v1.0/users` chỉ trả về 11 thuộc tính, dưới dạng Microsoft graph tự động chọn một bộ thuộc tính *người dùng* mặc định để trả về. Nếu bạn cần thuộc tính *người dùng* khác, hãy sử dụng $Select để chọn các thuộc tính nhu cầu ứng dụng của bạn. Dùng thử trong **Microsoft graph Explorer** trước tiên.

**Một số giá trị thuộc tính của người dùng là *null* ngay cả khi tôi biết chúng được đặt**

Giải thích có khả năng nhất là ứng dụng đã được cấp cho *người dùng. ReadBasic. tất cả* quyền. Điều này cho phép ứng dụng đọc một tập hợp các thuộc tính người dùng hạn chế, trả về tất cả các thuộc tính khác là NULL ngay cả khi họ đã thiết lập trước đó. Hãy thử cấp cho *người dùng ứng dụng. đọc. tất cả* quyền thay thế.

Để biết thêm thông tin, hãy xem quyền đối với [người dùng của Microsoft graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Tôi đang gặp sự cố khi sử dụng các tham số truy vấn OData để lọc dữ liệu trong yêu cầu của tôi**

Trong khi Microsoft graph hỗ trợ một phạm vi rộng của các tham số truy vấn OData, nhiều tham số trong số đó không được hỗ trợ đầy đủ bởi dịch vụ thư mục (các tài nguyên kế thừa từ *Directoryobject*) trong Microsoft graph. Những giới hạn tương tự được trình bày trong Azure AD graph vẫn tồn tại đối với hầu hết các phần trong Microsoft graph:

1. **Không được hỗ trợ**: $count, $search và $Filter trên các giá trị *null* hoặc *không phải là NULL*
2. **Không được hỗ trợ**: $Filter trên các thuộc tính nhất định (xem chủ đề tài nguyên mà bạn có thể lọc các thuộc tính nào)
3. **Không được hỗ trợ**: hoán trang, lọc và sắp xếp cùng lúc
4. **Không được hỗ trợ**: lọc trên mối quan hệ. Ví dụ-tìm tất cả các thành viên của nhóm kỹ thuật ở Vương Quốc Anh.
5. **Hỗ trợ một phần**: $orderby trên *người dùng* (DisplayName và userPrincipalName chỉ) và *nhóm*
6. **Hỗ trợ một phần**: $Filter (chỉ hỗ trợ các *EQ*, *Startswith*, *or* *và và* giới hạn *nào*) hỗ trợ, $Expand (mở rộng mối quan hệ của một đối tượng trả về tất cả mối quan hệ, nhưng mở rộng tập hợp mối quan hệ của đối tượng được giới hạn)

Để biết thêm thông tin, hãy xem [tùy chỉnh phản hồi với tham số truy vấn](https://docs.microsoft.com/graph/query-parameters).

**API tôi đang gọi không hoạt động-tôi có thể làm việc kiểm tra khác ở đâu?**

**Microsoft graph Explorer** -kiểm tra API đồ thị Microsoft trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu và cũng có thể xem các **truy vấn mẫu** trong Microsoft graph Explorer.

**Khi tôi truy vấn dữ liệu có vẻ như tôi nhận được thiết lập dữ liệu không đầy đủ**

Nếu bạn đang truy vấn một tuyển tập (như *người dùng*), Microsoft graph sẽ sử dụng giới hạn trang phía máy chủ để kết quả luôn được trả về bằng một kích cỡ trang mặc định. Ứng dụng của bạn sẽ luôn mong đợi đến trang thông qua các bộ sưu tập trả về từ dịch vụ.

Để biết thêm thông tin, hãy xem:

- [Các biện pháp tốt nhất của Microsoft graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Dữ liệu biểu đồ Microsoft phân trang trong ứng dụng của bạn](https://docs.microsoft.com/graph/paging)

**Ứng dụng của tôi quá chậm và cũng đang nhận được Throttled. Tôi có thể thực hiện những cải thiện nào?**

Tùy thuộc vào tình huống của bạn, có nhiều tùy chọn khác nhau trong việc xử lý của bạn để làm cho ứng dụng của bạn thêm performant, và trong một số trường hợp, ít dễ bị hơn là Throttled bởi dịch vụ (khi bạn đang thực hiện quá nhiều cuộc gọi).

Để tìm hiểu thêm, hãy xem:

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
