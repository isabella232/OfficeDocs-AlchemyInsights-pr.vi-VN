---
title: Các vấn đề về xác thực
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976871"
---
# <a name="authentication-issues"></a>Các vấn đề về xác thực

**Bạn đang tìm kiếm thông tin về các mã lỗi được trả về từ Azure Active Directory (Azure AD) dịch vụ mã thông báo bảo mật (STS)?** Xem [mã lỗi xác thực AZURE AD và ủy quyền](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) để tìm mô tả lỗi, bản sửa lỗi và một số giải pháp thay thế.

Lỗi ủy quyền có thể là kết quả của một số vấn đề khác nhau, phần lớn trong số đó tạo ra lỗi 401 hoặc 403. Ví dụ, các vấn đề sau đây có thể dẫn đến lỗi ủy quyền:

- [Dòng mua lại mã](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) thông báo không chính xác 
- Phạm vi [quyền](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) được đặt cấu hình kém 
- Thiếu sự [đồng ý](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Để giải quyết các lỗi ủy quyền phổ biến, hãy thử các bước được cung cấp bên dưới mà hầu hết khớp với lỗi mà bạn nhận được. Có thể áp dụng nhiều hơn một bước để có lỗi mà bạn nhận được.

**401 lỗi không được phép: là mã thông báo hợp lệ của bạn?**

Đảm bảo rằng ứng dụng của bạn đang trình bày mã thông báo truy nhập hợp lệ vào Microsoft graph như một phần của yêu cầu. Lỗi này thường có nghĩa là mã thông báo Access có thể bị thiếu trong phần đầu đề yêu cầu xác thực HTTP hoặc mã thông báo không hợp lệ hoặc đã hết hạn. Chúng tôi đặc biệt khuyên bạn nên sử dụng thư viện xác thực Microsoft (MSAL) để mua lại mã bản quyền truy nhập. Ngoài ra, lỗi này có thể xảy ra nếu bạn tìm cách sử dụng mã thông báo truy nhập được ủy quyền cho tài khoản Microsoft cá nhân để truy nhập API chỉ hỗ trợ tài khoản cơ quan hoặc trường học (tài khoản tổ chức).

**lỗi 403 bị cấm: bạn đã chọn tập hợp quyền?**

Đảm bảo rằng bạn đã yêu cầu tập hợp các quyền đúng dựa trên API của Microsoft graph, cuộc gọi ứng dụng của bạn. Các quyền tối thiểu được đề xuất-đặc quyền được cung cấp trong tất cả các chủ đề về phương pháp tham chiếu API của Microsoft graph. Ngoài ra, các quyền đó phải được cấp cho ứng dụng bởi người dùng hoặc người quản trị. Cấp quyền bình thường sẽ xảy ra thông qua một trang chấp thuận hoặc cách dùng lưỡi đăng ký ứng dụng Azure Portal. Từ lưỡi cưa **thiết đặt** cho ứng dụng, hãy bấm **quyền bắt buộc**, rồi bấm **cấp quyền**. Để biết thêm thông tin, hãy xem:

- [Quyền đối với đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) 
- [Tìm hiểu về quyền và sự đồng ý của Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**lỗi 403 bị lỗi: đã có ứng dụng của bạn có được một mã thông báo phù hợp với các quyền được chọn không?**

Đảm bảo rằng các loại quyền được yêu cầu hoặc cấp khớp với loại mã thông báo truy nhập mà ứng dụng của bạn đã mua lại. Bạn có thể yêu cầu và cấp quyền ứng dụng nhưng bằng cách sử dụng các thẻ dòng mã nguồn tương tác thay vì thẻ dòng chứng danh của máy khách, hoặc yêu cầu và cấp quyền ủy nhiệm nhưng dùng thẻ dòng chứng danh máy khách thay vì thẻ dòng mã được giao.

Để biết thêm thông tin liên quan đến việc mua thẻ, hãy xem:

- [Nhận quyền truy nhập thay mặt cho người dùng và quyền được giao](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 dòng mã ủy quyền](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Nhận quyền truy nhập mà không cần người dùng (Daemon Service) và quyền ứng dụng](https://docs.microsoft.com/graph/auth-v2-service) 
- [Dòng thông tin xác thực máy khách của Azure AD v 2.0-OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**lỗi 403 bị cấm: đặt lại mật khẩu**

Hiện tại, không có quyền ứng dụng dịch vụ đến dịch vụ cho phép đặt lại mật khẩu người dùng. Những API này chỉ được hỗ trợ bằng cách dùng mã được gán tương tác với người quản trị đã đăng nhập. Để biết thêm thông tin, hãy xem quyền đối với [Microsoft graph](https://docs.microsoft.com/graph/permissions-reference).

**403 bị cấm: người dùng có quyền truy nhập và chúng được cấp phép không?**

Đối với các dòng mã được giao, Microsoft graph đánh giá xem liệu yêu cầu đã được phép dựa trên các quyền được cấp cho ứng dụng và các quyền mà người dùng đã đăng nhập có. Thông thường, lỗi này cho biết người dùng không đủ đặc quyền để thực hiện yêu cầu **hoặc** người dùng không được cấp phép cho dữ liệu được truy nhập. Chỉ những người dùng có các quyền hoặc giấy phép bắt buộc có thể thực hiện các yêu cầu thành công.

**403 bị cấm: bạn đã chọn đúng API của tài nguyên?**

API các dịch vụ như kiểm tra đồ thị của Microsoft rằng các yêu cầu *AUD* (khán giả) trong mã thông báo Access đã nhận phù hợp với giá trị dự kiến chính nó, và nếu không, lỗi 403 bị cấm xảy ra. Lỗi phổ biến gây ra lỗi này đang cố gắng sử dụng mã thông báo đã mua cho các API của Azure AD graph, API Outlook hoặc SharePoint/OneDrive để gọi tới Microsoft graph (hoặc ngược lại). Đảm bảo rằng tài nguyên (hoặc phạm vi) ứng dụng của bạn sẽ có được mã thông báo cho khớp với API mà ứng dụng đang gọi.

**400 yêu cầu xấu hoặc 403 bị cấm: người dùng tuân thủ chính sách truy nhập có điều kiện của tổ chức của họ không?**

Dựa trên các chính sách truy nhập có điều kiện (CA) của tổ chức, người dùng sẽ truy nhập vào tài nguyên của Microsoft graph thông qua ứng dụng của bạn có thể bị thách thức để biết thêm thông tin không có trong ứng dụng Access của bạn được mua. Trong trường hợp này, ứng dụng của bạn sẽ nhận được **400 với lỗi *interaction_required*** trong quá trình mua lại mã bản quyền truy nhập hoặc **403 với *Insufficient_claims*** lỗi khi gọi đến Microsoft graph. Trong cả hai trường hợp, phản hồi lỗi chứa thông tin bổ sung mà có thể được trình bày vào điểm cuối được ủy quyền để thách thức người dùng để biết thêm thông tin (chẳng hạn như xác thực đa yếu tố hoặc đăng ký thiết bị).

Để biết thêm thông tin liên quan đến truy nhập có điều kiện, hãy xem:

- [Xử lý các thách thức truy nhập có điều kiện bằng MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Hướng dẫn về nhà phát triển cho Azure Active Directory điều kiện truy nhập](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and AZURE AD GRAPH API (đồ họa Bad)_* _

- Bắt đầu từ ngày 30 tháng 6, 2020, chúng tôi sẽ không còn thêm bất kỳ tính năng nào mới vào thư viện xác thực Azure Active Directory (ADAL) và Azure AD graph API (đồ họa Bad). Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.
- Bắt đầu từ ngày 30 tháng 6, 2022, chúng tôi sẽ kết thúc hỗ trợ đối với đồ thị ADAL và Bad và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.
    - Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào.
    - Ứng dụng bằng cách sử dụng đồ thị Bad sau khi thời gian này không còn nhận được phản hồi từ điểm cuối của biểu đồ.

*Di chuyển _ Adal**

Chúng tôi khuyên bạn nên cập nhật lên [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất. Đề xuất này nằm trong ngữ cảnh của Microsoft di chuyển các ứng dụng của mình sang MSAL bằng hạn chót cuối cùng hỗ trợ. Mục tiêu của việc di chuyển ứng dụng của Microsoft ' sang MSAL là đảm bảo rằng các ứng dụng được hưởng lợi từ bảo mật liên tục và cải thiện tính năng của MSAL.

- [Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn, và nếu có, hãy đến bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc ứng dụng. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.

**Di chuyển đồ thị trong Bad**

Đối với các ứng dụng đang sử dụng đồ thị Bad, hãy làm theo hướng dẫn của chúng tôi để [di chuyển các ứng dụng đồ thị AZURE AD sang Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad. Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào. Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn thông tin về việc sử dụng đồ thị trong toàn bộ đối tượng thuê của bạn.

 










