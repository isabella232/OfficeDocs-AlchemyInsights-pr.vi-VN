---
title: Khắc phục sự cố người dùng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: 0c4ee54a6f1d00e7fd3794539ba185afa4327af1124d8057550806f7fa87de7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092972"
---
# <a name="announcements"></a>Thông báo

Làm theo hướng dẫn của Google về việc kiểm tra tính tương thích để kiểm tra xem các ứng dụng của bạn có bị ảnh hưởng hay không. Hướng dẫn của Google có sẵn trong https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Đảm bảo bạn sử dụng dạng xem web hệ thống hoặc trình duyệt hệ thống khi đăng nhập người dùng bằng tài khoản Google dành cho người tiêu dùng. Để biết thêm thông tin, [hãy xem mục Sự cố đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)


**Tôi không thể tạo người dùng mới trong thư mục Azure AD của mình**

Để khắc phục sự cố về việc không thể tạo người dùng mới trong Azure AD, hãy thực hiện các bước sau đây:

1. Đảm bảo rằng bạn được phép tạo người dùng tiêu chuẩn mới. Chỉ người quản trị toàn cầu hoặc vai trò người quản trị người dùng trong Azure Active Directory (AD) mới có thể tạo người dùng chuẩn mới. Nếu bạn không ở trong một trong những vai trò này, hãy yêu cầu người quản trị thêm bạn vào một trong những vai trò này hoặc tạo tài khoản người dùng mới cho bạn.
2. Đảm bảo rằng tên người dùng nằm trong miền được xác minh trong Azure AD của bạn. Nếu bạn không có bất kỳ tên miền riêng đã xác minh nào trong Azure AD, bạn có thể sử dụng miền ban đầu Azure AD kết thúc bằng *.onmicrosoft.com.
3. Đảm bảo rằng tên người dùng nằm trong miền không được liên kết với Azure AD từ AD tại chỗ của bạn. Không thể thêm người dùng vào đám mây với các tên miền được liên kết từ tại chỗ.
4. Đảm bảo rằng không có người dùng hoặc liên hệ nào khác đã có tên người dùng mà bạn muốn gán cho người dùng mới. Tên người dùng phải là duy nhất trong Azure AD.
5. Hãy [xem mục Vai trò và người quản trị Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) cho Azure AD của bạn.
6. Xem các [tên miền cho](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) Azure AD của bạn.
7. Xem [lại Nhật ký kiểm tra](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) để xem thông tin chi tiết hơn về người dùng được tạo hoặc xóa gần đây như người đã thực hiện hành động và thời điểm thực hiện hành động.
8. Để biết thêm thông tin về cách thêm người dùng mới, hãy [xem mục Sử dụng cổng thông tin Azure để tạo người dùng mới trong Azure AD của bạn.](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
9. Để biết thêm thông tin về các quyền vai trò của người quản trị trong Azure AD, hãy [xem mục Vai trò quản trị Azure AD.](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
10. Để biết chi tiết về cách tạo người dùng đang sử dụng Azure AD Powershell, hãy [xem Azure AD PowerShell để tạo người dùng mới.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)

**Sự cố với đăng ký tự phục vụ**

Để khắc phục sự cố về đăng ký tự phục vụ, hãy thực hiện các bước sau đây:

1. Để sử dụng đăng ký tự phục vụ với ứng dụng của bạn, trước tiên hãy cho phép đăng ký tự phục vụ cho đối tượng thuê của bạn. 
2. Để cho phép ứng dụng hỗ trợ đăng ký tự phục vụ, hãy thêm ứng dụng đó vào dòng người dùng của bạn. Lần tới khi bạn đi tới trang đăng nhập của ứng dụng đó, bạn sẽ thấy tùy chọn Không ***có tài khoản? Hãy tạo tài khoản!***. Điều này sẽ bắt đầu quy trình đăng ký tự phục vụ.
3. Để biết thông tin về cách sử dụng đăng ký tự phục vụ để nhập thông tin cho một tổ chức trong Azure AD, hãy xem mục Đăng ký [tự phục vụ cho Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Sau khi liên kết dòng người dùng với một hoặc nhiều ứng dụng, người dùng truy nhập ứng dụng đó sẽ có thể đăng ký và có được tài khoản khách bằng các tùy chọn được đặt cấu hình trong dòng người dùng. Để biết thêm thông tin về việc đăng ký và lấy tài khoản khách, người dùng có thể xem mục Đăng ký tự [phục vụ cho người dùng khách.](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)

**Sự cố khi mời người dùng bên ngoài**

Để khắc phục sự cố liên quan đến việc mời người dùng bên ngoài, hãy thực hiện bước sau đây:

Đảm bảo rằng bạn gửi thư mời của người dùng đến địa chỉ email khớp với tên mà người dùng đăng nhập. Nếu bạn gửi lời mời đến địa chỉ email proxy của người dùng, người dùng không thể lấy lại nó. Để biết thêm thông tin, hãy [xem mục Hướng dẫn sử dụng Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/)

**Tôi không thể gán giấy phép cho người dùng**

Để khắc phục sự cố về việc gán giấy phép cho người dùng, hãy thực hiện các bước sau đây:

1. Để quản lý giấy phép người dùng, hãy đảm bảo rằng bạn sử dụng tài khoản với một trong các vai trò người quản trị bắt buộc: người quản trị toàn cầu, người quản trị giấy phép hoặc người quản trị người dùng. Bạn có thể kiểm tra vai trò của người dùng trong tab **Vai trò thư** mục trên lưỡi người dùng.
2. Nếu bạn đang sử dụng cổng thông tin Và gán giấy phép Azure không thành công, hãy bấm vào thông báo ở góc trên bên phải. Làm như vậy sẽ mở một chiếc lưỡi với chi tiết về sự cố xảy ra. Trong hầu hết các trường hợp, đủ hiểu và giải quyết sự cố.
3. Trước khi có thể gán giấy phép cho người dùng, hãy đảm bảo rằng thuộc **tính Vị trí** Sử dụng được đặt cho người dùng. Xác minh người dùng đã đặt thuộc tính đó bằng cách xem tab **Hồ** sơ trên lưỡi người dùng.
4. Đảm bảo có đủ giấy phép sẵn dùng cho sản phẩm mà bạn đang tìm cách gán. Bạn có thể xem số giấy phép khả dụng trong cổng thông tin Azure, tại Azure Active Directory -> giấy phép [-> Tất cả sản phẩm.](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)
5. Người dùng có thể đã có giấy phép khác có các dịch vụ xung đột với những giấy phép mới mà bạn đang tìm cách gán. Ví dụ: nếu người dùng đã bật dịch vụ Exchange Online (Plan 1), bạn sẽ không thể gán giấy phép với giấy phép đó Exchange Online (Plan 2). Vô hiệu hóa một trong các dịch vụ để cho phép gán giấy phép mới. Nếu bạn đang sử dụng cổng thông tin Azure  hoặc lệnh ghép ngắn PowerShell, trang chi tiết vấn đề sẽ liệt kê các dịch vụ cụ thể đang gây ra xung đột.
6. Nếu bạn đang tìm cách loại bỏ giấy phép và điều đó không thành công, người dùng có thể có giấy phép khác với các dịch vụ phụ thuộc vào các dịch vụ mà bạn đang tìm cách loại bỏ. Nếu bạn đang sử dụng cổng thông tin Azure hoặc lệnh ghép ngắn PowerShell, thông báo lỗi sẽ liệt kê các dịch vụ cụ thể có các phụ thuộc.
7. Nếu bạn muốn hiểu tại sao giấy phép đã được thêm/loại bỏ khỏi người dùng (ví dụ: những người khác trong tổ chức của bạn có thể đã thực hiện thay đổi), hãy kiểm tra nhật ký kiểm tra. Đặt bộ lọc thành các **hoạt động cấp** phép để hiển thị tất cả sửa đổi, bao gồm cả "chủ động" đã thực hiện chúng.
8. Nếu bạn đang sử dụng Exchange Online, một số người dùng trong đối tượng thuê của bạn có thể được cấu hình không chính xác với cùng một giá trị địa chỉ proxy. Trong những trường hợp đó, bạn có thể thấy thông báo lỗi chung khi thao tác giấy phép không thành công. [Bài viết này](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) có chứa thêm thông tin về sự cố này, bao gồm thông tin về cách kết nối [với Exchange Online cách sử dụng PowerShell từ xa.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) Để xác định người dùng nào trong đối tượng thuê của bạn, hãy thực hiện lệnh ghép ngắn Exchange Online như sau:

Chạy

Get-Recipient | trong đó {$_. EmailAddresses -match <user principal name> } | fL Name, RecipientType,emailaddresses





