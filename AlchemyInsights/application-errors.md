---
title: Lỗi ứng dụng
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
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984653"
---
# <a name="application-errors"></a>Lỗi ứng dụng

Bạn đang tìm thông tin về các **mã lỗi** được trả về từ Azure Active Directory (Azure AD) dịch vụ mã thông báo bảo mật (STS)? Đọc tính năng [xác thực AZURE AD và các mã lỗi ủy quyền](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) để tìm các mô tả lỗi, bản sửa lỗi và một số giải pháp thay thế được gợi ý.

Lỗi ủy quyền có thể là kết quả của một số vấn đề khác nhau, phần lớn trong số đó tạo ra lỗi 401 hoặc 403. Ví dụ, các thao tác sau có thể dẫn đến lỗi ủy quyền:

- [Dòng mua lại mã](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) thông báo không chính xác 
- Phạm vi [quyền](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) được đặt cấu hình kém 
- Thiếu sự [đồng ý](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Để giải quyết các lỗi ủy quyền phổ biến, hãy thử các bước được cung cấp bên dưới mà hầu hết các khớp với lỗi mà bạn nhận được. Có thể áp dụng nhiều hơn một.

**401 lỗi không được phép: là mã thông báo hợp lệ của bạn?**

Đảm bảo rằng ứng dụng của bạn đang trình bày mã thông báo truy nhập hợp lệ vào Microsoft graph như một phần của yêu cầu. Lỗi này thường có nghĩa là mã thông báo Access có thể bị thiếu trong phần đầu đề yêu cầu xác thực HTTP hoặc mã thông báo không hợp lệ hoặc đã hết hạn. Chúng tôi đặc biệt khuyên bạn nên sử dụng [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) để mua lại mã bản quyền truy nhập. Ngoài ra, lỗi này có thể xảy ra nếu bạn tìm cách sử dụng mã thông báo truy nhập được ủy quyền cho tài khoản Microsoft cá nhân để truy nhập API chỉ hỗ trợ tài khoản cơ quan hoặc trường học (tài khoản tổ chức).

**lỗi 403 bị cấm: bạn đã chọn tập hợp quyền?**

Kiểm tra xem bạn đã yêu cầu tập hợp quyền chính xác dựa trên API của Microsoft graph, cuộc gọi ứng dụng của bạn hay không. Các quyền đặc quyền nhất định được cung cấp trong tất cả các chủ đề về phương pháp tham chiếu API của Microsoft graph. Ngoài ra, các quyền đó phải được cấp cho ứng dụng bởi người dùng hoặc người quản trị. Cấp quyền bình thường sẽ xảy ra thông qua một trang chấp thuận hoặc bằng cách cấp quyền sử dụng lưỡi đăng ký ứng dụng Azure Portal. Từ lưỡi cưa **thiết đặt** cho ứng dụng, hãy bấm **quyền bắt buộc**, rồi bấm **cấp quyền**.

- [Quyền đối với đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Tìm hiểu về quyền và sự đồng ý của Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**lỗi 403 bị lỗi: đã có ứng dụng của bạn có được một mã thông báo phù hợp với các quyền được chọn không?**

Hãy đảm bảo rằng loại quyền được yêu cầu hoặc cấp khớp với loại mã thông báo truy nhập mà ứng dụng của bạn đã mua lại. Bạn có thể yêu cầu và cấp quyền ứng dụng nhưng bằng cách sử dụng các thẻ dòng mã nguồn tương tác thay vì thẻ dòng chứng danh của máy khách, hoặc yêu cầu và cấp quyền ủy nhiệm nhưng dùng thẻ dòng chứng danh của máy tính thay vì các thẻ dòng mã nguồn được giao.

- [Nhận quyền truy nhập thay mặt cho người dùng và quyền được giao](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 dòng mã ủy quyền](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Nhận quyền truy nhập mà không cần người dùng (Daemon Service) và quyền ứng dụng](https://docs.microsoft.com/graph/auth_v2_service) 
- [Dòng thông tin xác thực máy khách của Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**lỗi 403 bị cấm: đặt lại mật khẩu**

Hiện tại, không có quyền ứng dụng dịch vụ đến dịch vụ cho phép đặt lại mật khẩu người dùng. Những API này chỉ được hỗ trợ bằng cách dùng mã được gán tương tác với người quản trị đã đăng nhập.

- [Quyền đối với đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference)

**403 bị cấm: người dùng có quyền truy nhập và chúng được cấp phép không?**

Đối với các dòng mã được giao, Microsoft graph đánh giá nếu yêu cầu được phép dựa trên các quyền được cấp cho ứng dụng và các quyền mà người dùng đã đăng nhập có. Thông thường, lỗi này cho biết người dùng không đủ đặc quyền để thực hiện yêu cầu hoặc người dùng không được cấp phép cho dữ liệu được truy nhập. Chỉ những người dùng có các quyền hoặc giấy phép bắt buộc có thể thực hiện các yêu cầu thành công.

**403 bị cấm: bạn đã chọn đúng API của tài nguyên?**

API các dịch vụ như kiểm tra đồ thị của Microsoft rằng yêu cầu AUD (khán giả) trong mã thông báo Access đã nhận phù hợp với giá trị dự kiến chính nó và nếu không, nó sẽ kết quả trong lỗi 403 bị cấm. Lỗi phổ biến gây ra lỗi này đang cố gắng sử dụng mã thông báo đã mua cho các API của Azure AD graph, API Outlook hoặc SharePoint/OneDrive để gọi tới Microsoft graph (hoặc ngược lại). Đảm bảo rằng tài nguyên (hoặc phạm vi) ứng dụng của bạn sẽ có được mã thông báo cho khớp với API mà ứng dụng đang gọi.

**400 yêu cầu xấu hoặc 403 bị cấm: người dùng tuân thủ chính sách truy nhập có điều kiện của tổ chức của họ không?**

Dựa trên các chính sách CA của tổ chức, người dùng truy nhập tài nguyên của Microsoft graph thông qua ứng dụng của bạn có thể bị thách thức để biết thông tin bổ sung không có trong Access mã thông báo ứng dụng của bạn ban đầu được mua. Trong trường hợp này, ứng dụng của bạn sẽ nhận được 400 với lỗi *interaction_required* trong quá trình mua lại mã bản quyền truy nhập hoặc 403 với *insufficient_claims* lỗi khi gọi đến Microsoft graph. Trong cả hai trường hợp, phản hồi lỗi có chứa thông tin bổ sung mà có thể được trình bày vào điểm cuối ủy quyền để thách thức người dùng để biết thêm thông tin (chẳng hạn như xác thực đa yếu tố hoặc đăng ký thiết bị).

- [Xử lý các thách thức truy nhập có điều kiện bằng MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Hướng dẫn về nhà phát triển cho Azure Active Directory điều kiện truy nhập](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
