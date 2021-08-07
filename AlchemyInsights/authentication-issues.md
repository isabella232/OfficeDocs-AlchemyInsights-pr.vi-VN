---
title: Sự cố xác thực
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
ms.openlocfilehash: c7e6d96940f8d7052ee4b49b22c0d1d7d5bd5f9277f4a7eff709def1da2e13af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019530"
---
# <a name="authentication-issues"></a>Sự cố xác thực

**Bạn đang tìm kiếm thông tin về mã lỗi AADSTS được trả về từ dịch vụ mã thông báo bảo mật (Azure AD) Azure Active Directory (STS)?** Hãy [xem mục Xác thực Azure AD và](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) mã lỗi ủy quyền để tìm mô tả lỗi AADSTS, các bản sửa lỗi và một số giải pháp thay thế được đề xuất.

Lỗi ủy quyền có thể là kết quả của một số sự cố khác nhau, đa số các lỗi gây ra lỗi 401 hoặc 403. Ví dụ: tất cả các sự cố sau đều có thể dẫn đến lỗi ủy quyền:

- Quy trình [thu thập mã thông báo truy nhập không chính xác](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Phạm vi quyền được đặt [cấu hình kém](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- Thiếu sự chấp [thuận](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

Để giải quyết các lỗi ủy quyền phổ biến, hãy thử các bước được cung cấp dưới đây, phù hợp nhất với lỗi bạn đang nhận được. Nhiều bước có thể áp dụng cho lỗi mà bạn đang gặp phải.

**401 Lỗi trái phép: Mã thông báo của bạn có hợp lệ không?**

Đảm bảo rằng ứng dụng của bạn đang trình bày một mã thông báo truy nhập hợp lệ cho Microsoft Graph như là một phần của yêu cầu. Lỗi này thường có nghĩa là mã thông báo truy nhập có thể bị thiếu trong tiêu đề yêu cầu xác thực HTTP hoặc mã thông báo không hợp lệ hoặc đã hết hạn. Chúng tôi khuyên bạn nên sử dụng Thư viện Xác thực Microsoft (MSAL) để mua mã thông báo truy nhập. Ngoài ra, lỗi này có thể xảy ra nếu bạn tìm cách sử dụng mã thông báo truy nhập được ủy quyền cấp cho tài khoản Microsoft cá nhân để truy nhập API chỉ hỗ trợ tài khoản cơ quan hoặc trường học (tài khoản tổ chức).

**403 Lỗi cấm: Bạn đã chọn tập hợp quyền phù hợp chưa?**

Đảm bảo rằng bạn đã yêu cầu tập hợp quyền chính xác dựa trên API Microsoft Graph gọi ứng dụng của bạn. Các quyền có đặc quyền tối thiểu được đề xuất sẽ được cung cấp trong tất cả các chủ đề phương pháp tham Graph API của Microsoft Graph. Ngoài ra, người dùng hoặc người quản trị phải cấp các quyền đó cho ứng dụng. Việc cấp quyền thường xảy ra thông qua trang đồng ý hoặc sử dụng lưỡi đăng ký ứng dụng Cổng thông tin Azure. Từ **lưỡi Cài đặt** của ứng dụng, bấm vào Quyền **Bắt** buộc , rồi bấm vào **Cấp Quyền.** Để biết thêm thông tin, hãy xem:

- [Quyền đối Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) 
- [Hiểu về các quyền và sự chấp thuận Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Lỗi cấm: Ứng dụng của bạn có nhận được mã thông báo khớp với các quyền đã chọn không?**

Đảm bảo rằng các loại quyền được yêu cầu hoặc cấp khớp với loại mã thông báo truy nhập mà ứng dụng của bạn mua được. Có thể bạn đang yêu cầu và cấp quyền của ứng dụng nhưng sử dụng mã thông báo dòng mã tương tác được ủy nhiệm thay vì mã thông tin xác thực máy khách, hoặc yêu cầu và cấp quyền được ủy nhiệm nhưng sử dụng mã thông tin xác thực máy khách thay vì các mã thông báo dòng mã ủy nhiệm.

Để biết thêm thông tin liên quan đến việc mua mã thông báo, hãy xem:

- [Nhận quyền truy nhập thay mặt người dùng và các quyền được ủy nhiệm](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - Dòng mã ủy quyền OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Nhận quyền truy nhập mà không có người dùng (dịch vụ daemon) và quyền ứng dụng](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - Dòng thông tin xác thực máy khách OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Lỗi cấm: Đặt lại mật khẩu**

Hiện tại, không có quyền đối với dịch vụ daemon đối với dịch vụ mà không cho phép đặt lại mật khẩu người dùng. Các API này chỉ được hỗ trợ sử dụng các dòng mã đại diện tương tác với người quản trị đã đăng nhập. Để biết thêm thông tin, [hãy xem mục Quyền Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference).

**403 Cấm: Người dùng có quyền truy nhập và được cấp phép không?**

Đối với các dòng mã được ủy quyền, Microsoft Graph đánh giá xem yêu cầu đó có được cho phép hay không dựa trên các quyền cấp cho ứng dụng và các quyền mà người dùng đã đăng nhập có. Thông thường, lỗi này cho biết người dùng  không có đặc quyền để thực hiện yêu cầu hoặc người dùng không được cấp phép cho dữ liệu đang được truy nhập. Chỉ những người dùng có quyền hoặc giấy phép bắt buộc mới có thể thực hiện thành công yêu cầu đó.

**403 Cấm: Bạn có chọn đúng API tài nguyên không?**

Các dịch vụ API như Microsoft  Graph kiểm tra xem yêu cầu đối tượng (người xem) trong mã thông báo truy nhập đã nhận có khớp với giá trị dự kiến cho chính nó không và nếu không khớp thì sẽ xảy ra lỗi 403 Cấm. Một lỗi phổ biến dẫn đến lỗi này là việc tìm cách sử dụng mã thông báo mua được cho Azure AD Graph, API Outlook hoặc api SharePoint/OneDrive để gọi là API Microsoft Graph (hoặc ngược lại). Đảm bảo rằng tài nguyên (hoặc phạm vi) ứng dụng của bạn đang lấy mã thông báo để khớp với API mà ứng dụng đang gọi.

**400 Yêu cầu Xấu hoặc 403 Bị cấm: Người dùng có tuân thủ các chính sách truy nhập có điều kiện (CA) của tổ chức họ không?**

Dựa trên các chính sách truy nhập có điều kiện (CA) của một tổ chức, người dùng truy nhập các tài nguyên Microsoft Graph thông qua ứng dụng của bạn có thể bị thách thức đối với thông tin bổ sung không có trong mã thông báo truy nhập mà ứng dụng của bạn thu được từ đầu. Trong trường hợp này, ứng dụng của bạn nhận được **lỗi 400** cùng với lỗi interaction_required trong quá trình mua mã thông báo truy nhập hoặc lỗi **403 *insufficient_claims*** khi gọi cho Microsoft Graph. Trong cả hai trường hợp, phản hồi lỗi chứa thông tin bổ sung có thể được trình bày cho điểm cuối được ủy quyền để thách thức người dùng về các thông tin bổ sung (như xác thực đa yếu tố hoặc đăng ký thiết bị).

Để biết thêm thông tin liên quan đến truy nhập có điều kiện, hãy xem:

- [Xử lý các thách thức truy nhập có điều kiện bằng msal](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Hướng dẫn dành cho nhà phát triển Azure Active Directory nhập có điều kiện](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

***Kết thúc hỗ trợ cho Azure Active Directory Thư viện Xác thực (ADAL) và API Graph Azure AD (AAD Graph)***

- Kể từ ngày 30 tháng 6 năm 2020, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Thư viện Xác thực Azure Active Directory (ADAL) và Azure AD Graph API (AAD Graph). Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và cập nhật bảo mật nhưng sẽ không cung cấp các bản cập nhật tính năng nữa.
- Bắt đầu từ ngày 30 tháng 6 năm 2022, chúng tôi sẽ kết thúc hỗ trợ cho ADAL và AAD Graph và sẽ không cung cấp hỗ trợ kỹ thuật hay cập nhật bảo mật nữa.
    - Ứng dụng sử dụng ADAL trên các phiên bản HĐH hiện có sẽ tiếp tục hoạt động sau thời gian này nhưng sẽ không nhận được bất kỳ hỗ trợ kỹ thuật hay bản cập nhật bảo mật nào.
    - Các ứng dụng sử dụng AAD Graph sau thời gian này có thể không còn nhận được phản hồi từ điểm cuối của AAD Graph khác.

**Di chuyển ADAL**

Chúng tôi khuyên bạn nên cập nhật [lên Thư viện Xác thực Microsoft (MSAL),](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)nơi có các tính năng và bản cập nhật bảo mật mới nhất. Đề xuất này nằm trong bối cảnh Microsoft di chuyển các ứng dụng sang MSAL trước hạn chót kết thúc hỗ trợ. Mục tiêu di chuyển của các ứng dụng Microsoft sang MSAL là nhằm đảm bảo rằng các ứng dụng này được hưởng lợi từ các cải thiện liên tục về bảo mật và tính năng của MSAL.

- [Đọc Câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Tìm hiểu về cách di chuyển ứng dụng trên cơ sở từng nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Nếu bạn cần trợ giúp để hiểu rõ ứng dụng nào sử dụng ADAL, chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có thể, hãy liên hệ với bất kỳ nhà cung cấp phần mềm độc lập (ISV) hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn danh sách tất cả các ứng dụng không phải ADAL của Microsoft trong đối tượng thuê của bạn.

**Di chuyển thiết Graph AAD**

Đối với các ứng dụng đang sử dụng AAD Graph, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng [Azure AD Graph sang Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true)

- [Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist) 
- Cổng thông tin đăng ký ứng dụng Azure của bạn hiển thị các ứng dụng đang sử dụng AAD Graph. Chúng tôi khuyên bạn nên xem lại tất cả mã nguồn của ứng dụng và nếu có, hãy liên hệ với bất kỳ ISV hoặc nhà cung cấp ứng dụng nào. Bộ trợ giúp của Microsoft cũng có thể cung cấp cho bạn thông tin về toàn bộ mức sử dụng AAD Graph đối tượng thuê của bạn.

 










