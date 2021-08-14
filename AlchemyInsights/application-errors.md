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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931471"
---
# <a name="application-errors"></a>Lỗi ứng dụng

Bạn đang tìm kiếm thông tin về mã lỗi **AADSTS** được trả về từ dịch vụ mã thông báo bảo mật Azure Active Directory (Azure AD) (STS)? Đọc [mục Xác thực Azure AD và](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) mã lỗi ủy quyền để tìm mô tả lỗi AADSTS, các bản sửa lỗi và một số giải pháp thay thế được đề xuất.

Lỗi ủy quyền có thể là kết quả của một số sự cố khác nhau, đa số các lỗi gây ra lỗi 401 hoặc 403. Ví dụ: tất cả những điều sau đây đều có thể dẫn đến lỗi ủy quyền:

- Quy trình [thu thập mã thông báo truy nhập không chính xác](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Phạm vi quyền được đặt [cấu hình kém](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- Thiếu sự chấp [thuận](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

Để giải quyết các lỗi ủy quyền phổ biến, hãy thử các bước được cung cấp dưới đây gần nhất với lỗi mà bạn đang nhận được. Nhiều hơn một có thể áp dụng.

**401 Lỗi trái phép: Mã thông báo của bạn có hợp lệ không?**

Đảm bảo rằng ứng dụng của bạn đang trình bày một mã thông báo truy nhập hợp lệ cho Microsoft Graph như một phần của yêu cầu. Lỗi này thường có nghĩa là mã thông báo truy nhập có thể bị thiếu trong tiêu đề yêu cầu xác thực HTTP hoặc mã thông báo không hợp lệ hoặc đã hết hạn. Chúng tôi khuyên bạn nên sử dụng Thư viện Xác [thực Microsoft (MSAL) để](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) mua mã thông báo truy nhập. Ngoài ra, lỗi này có thể xảy ra nếu bạn tìm cách sử dụng mã thông báo truy nhập được ủy quyền cấp cho tài khoản Microsoft cá nhân để truy nhập API chỉ hỗ trợ tài khoản cơ quan hoặc trường học (tài khoản tổ chức).

**403 Lỗi cấm: Bạn đã chọn tập hợp quyền phù hợp chưa?**

Kiểm tra xem bạn đã yêu cầu tập hợp quyền chính xác dựa trên API Microsoft Graph gọi ứng dụng của bạn hay chưa. Các quyền có đặc quyền tối thiểu được đề xuất đều được cung cấp trong tất cả các chủ đề phương pháp tham khảo API Graph Microsoft Graph. Ngoài ra, người dùng hoặc người quản trị phải cấp các quyền đó cho ứng dụng. Việc cấp quyền thường xảy ra thông thường thông qua trang đồng ý hoặc bằng cách cấp quyền bằng cách sử dụng lưỡi đăng ký ứng dụng Cổng thông tin Azure. Từ **lưỡi Cài đặt** của ứng dụng, bấm vào Quyền **Bắt** buộc , rồi bấm vào **Cấp Quyền.**

- [Quyền đối Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference) 
- [Hiểu về các quyền và sự chấp thuận Azure AD](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Lỗi cấm: Ứng dụng của bạn có nhận được mã thông báo khớp với các quyền đã chọn không?**

Đảm bảo rằng loại quyền được yêu cầu hoặc cấp khớp với loại mã thông báo truy nhập mà ứng dụng của bạn mua được. Có thể bạn đang yêu cầu và cấp quyền ứng dụng nhưng sử dụng mã thông báo dòng mã tương tác được ủy nhiệm thay vì mã thông tin xác thực máy khách, hoặc yêu cầu và cấp quyền được ủy nhiệm nhưng sử dụng mã thông tin xác thực máy khách thay vì các mã thông báo dòng mã ủy nhiệm.

- [Nhận quyền truy nhập thay mặt người dùng và các quyền được ủy nhiệm](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - Dòng mã ủy quyền OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Nhận quyền truy nhập mà không có người dùng (dịch vụ daemon) và quyền ứng dụng](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - Dòng thông tin xác thực máy khách OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Lỗi cấm: Đặt lại mật khẩu**

Hiện tại, không có quyền đối với dịch vụ daemon đối với dịch vụ mà không cho phép đặt lại mật khẩu người dùng. Các API này chỉ được hỗ trợ sử dụng các dòng mã đại diện tương tác với người quản trị đã đăng nhập.

- [Quyền đối Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference)

**403 Cấm: Người dùng có quyền truy nhập và được cấp phép không?**

Đối với các dòng mã được ủy nhiệm, Microsoft Graph sẽ đánh giá xem yêu cầu có được cho phép dựa trên các quyền cấp cho ứng dụng và các quyền mà người dùng đã đăng nhập có. Thông thường, lỗi này cho biết người dùng không có đặc quyền để thực hiện yêu cầu hoặc người dùng không được cấp phép cho dữ liệu đang được truy nhập. Chỉ những người dùng có quyền hoặc giấy phép bắt buộc mới có thể thực hiện thành công yêu cầu đó.

**403 Cấm: Bạn có chọn đúng API tài nguyên không?**

Các dịch vụ API như Microsoft Graph kiểm tra xem yêu cầu đối tượng (người xem) trong mã thông báo truy nhập đã nhận có khớp với giá trị dự kiến cho chính nó không và nếu không khớp thì sẽ dẫn đến lỗi 403 Cấm. Một lỗi phổ biến dẫn đến lỗi này là việc tìm cách sử dụng mã thông báo mua được cho Azure AD Graph, API Outlook hoặc api SharePoint/OneDrive để gọi là API Microsoft Graph (hoặc ngược lại). Đảm bảo rằng tài nguyên (hoặc phạm vi) ứng dụng của bạn đang lấy mã thông báo để khớp với API mà ứng dụng đang gọi.

**400 Yêu cầu Xấu hoặc 403 Bị cấm: Người dùng có tuân thủ các chính sách truy nhập có điều kiện (CA) của tổ chức họ không?**

Based on an organization's CA policies, a user accessing Microsoft Graph resources via your app may be challenged for additional information that is not present in the access token your app originally acquired. Trong trường hợp này, ứng dụng của bạn nhận được lỗi 400 cùng với *lỗi interaction_required* trong quá trình mua mã thông báo truy nhập hoặc lỗi 403 *insufficient_claims* xảy ra khi gọi cho Microsoft Graph. Trong cả hai trường hợp, phản hồi lỗi chứa thông tin bổ sung có thể được trình bày cho điểm cuối được ủy quyền để thách thức người dùng về các thông tin bổ sung (như xác thực đa yếu tố hoặc đăng ký thiết bị).

- [Xử lý các thách thức truy nhập có điều kiện bằng msal ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Hướng dẫn dành cho nhà phát triển Azure Active Directory nhập có điều kiện](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
