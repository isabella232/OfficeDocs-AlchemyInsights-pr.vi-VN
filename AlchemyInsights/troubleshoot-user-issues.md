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
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901343"
---
# <a name="announcements"></a>Bố

Hãy làm theo hướng dẫn của Google về tính tương thích kiểm tra để kiểm tra xem các ứng dụng của bạn có bị ảnh hưởng không. Hướng dẫn của Google sẵn dùng https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Đảm bảo bạn sử dụng trình duyệt hệ thống WebView hoặc hệ thống khi đăng nhập vào người dùng của bạn với các tài khoản Google dành cho người dùng. Để biết thêm thông tin, hãy xem các [vấn đề đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Tôi không thể tạo người dùng mới trong thư mục Azure AD của tôi**

Để khắc phục sự cố không thể tạo người dùng mới trong Azure AD, hãy thực hiện các bước sau đây:

1. Đảm bảo rằng bạn được ủy quyền để tạo một người dùng tiêu chuẩn mới. Chỉ người quản trị toàn cầu hoặc vai trò người quản trị người dùng trong Azure Active Directory (AD) có thể tạo một người dùng chuẩn mới. Nếu bạn không ở trong một trong những vai trò này, hãy yêu cầu người quản trị thêm bạn vào một trong những vai trò này hoặc để tạo tài khoản người dùng mới cho bạn.
2. Đảm bảo rằng tên người dùng đang ở trong một tên miền được xác minh trong Azure AD của bạn. Nếu bạn không có bất kỳ tên miền riêng nào được xác minh trong Azure AD, bạn có thể sử dụng tên miền Azure AD ban đầu của bạn, kết thúc bằng *. onmicrosoft.com.
3. Đảm bảo rằng tên người dùng đang ở trong một tên miền không được liên kết với Azure AD từ quảng cáo tại cơ sở của bạn. Người dùng không thể được thêm vào điện toán đám mây có tên miền được liên kết từ tại cơ sở.
4. Đảm bảo rằng không có người dùng hoặc liên hệ nào khác đã có tên người dùng mà bạn muốn gán cho người dùng mới. Tên người dùng phải là duy nhất trên Azure AD.
5. Xem các [vai trò và người quản trị AZURE AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) cho Azure AD của bạn.
6. Xem [tên miền](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) cho Azure AD của bạn.
7. Xem lại [Nhật ký kiểm](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) tra để xem thông tin chi tiết hơn về một người dùng đã tạo hoặc đã xóa gần đây như những người thực hiện hành động và khi nào.
8. Để biết thêm thông tin về cách thêm người dùng mới, hãy xem [sử dụng cổng thông tin Azure để tạo người dùng mới trong AZURE AD của bạn](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Để biết thêm thông tin về quyền vai trò người quản trị trong Azure AD, hãy xem các [vai trò quản trị AZURE AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Để biết chi tiết về việc tạo một người dùng bằng cách sử dụng Azure AD PowerShell, hãy xem [AZURE AD PowerShell để tạo người dùng mới](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Sự cố với đăng ký tự phục vụ**

Để khắc phục sự cố về việc đăng ký tự phục vụ, hãy thực hiện các bước sau đây:

1. Để sử dụng tính năng đăng ký tự phục vụ với các ứng dụng của bạn, trước tiên, cho phép đăng ký tự phục vụ cho đối tượng thuê của bạn. 
2. Để kích hoạt ứng dụng để hỗ trợ đăng ký tự phục vụ, hãy thêm nó vào dòng người dùng của bạn. Lần tiếp theo bạn đi đến trang đăng nhập cho ứng dụng đó, bạn sẽ thấy một tùy chọn **_không có tài khoản? Tạo một!_* _. Thao số này sẽ khởi động quy trình đăng ký tự phục vụ.
3. Để biết thêm thông tin về cách sử dụng tính năng đăng ký tự phục vụ để thành lập một tổ chức trong Azure AD, hãy xem [đăng ký tự phục vụ cho AZURE AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Sau khi bạn liên kết dòng người dùng với một hoặc nhiều ứng dụng, những người dùng truy nhập ứng dụng đó sẽ có thể đăng ký và giành được tài khoản khách bằng cách dùng tùy chọn được đặt cấu hình trong dòng người dùng. Để biết thêm thông tin về việc đăng ký và đạt được tài khoản khách, người dùng có thể thấy [đăng ký tự phục vụ cho người dùng khách](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Vấn đề mời người dùng bên ngoài**

Để khắc phục sự cố về việc mời người dùng bên ngoài, hãy thực hiện bước sau đây:

Đảm bảo rằng bạn gửi lời mời của người dùng đến địa chỉ email khớp với tên mà người dùng đăng nhập. Nếu bạn gửi lời mời đến địa chỉ email proxy của người dùng, thì người dùng này không thể chuộc lại. Để biết thêm thông tin, hãy xem [tài liệu AZURE AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Tôi không thể gán giấy phép cho người dùng**

Để khắc phục sự cố về việc gán giấy phép cho người dùng, hãy thực hiện các bước sau đây:

1. Để quản lý giấy phép người dùng, hãy đảm bảo rằng bạn sử dụng tài khoản với một trong các vai trò người quản trị bắt buộc: người quản trị toàn cầu, người quản trị giấy phép hoặc người quản trị người dùng. Bạn có thể kiểm tra vai trò của người dùng trong tab **vai trò thư mục** trên lưỡi người dùng.
2. Nếu bạn đang sử dụng cổng thông tin Azure và gán giấy phép, hãy bấm vào thông báo ở góc trên bên phải. Thao động này sẽ mở ra một lưỡi với các chi tiết về những điều đã xảy ra. Trong hầu hết các trường hợp đủ để hiểu và giải quyết được sự cố.
3. Trước khi có thể gán giấy phép cho người dùng, hãy đảm bảo rằng thuộc tính **vị trí sử dụng** được đặt cho người dùng. Xác nhận người dùng đã thiết lập thuộc tính bằng cách xem tab **hồ sơ** trên lưỡi người dùng.
4. Đảm bảo có đủ giấy phép sẵn dùng cho sản phẩm mà bạn đang cố gắng gán. Bạn có thể xem số lượng giấy phép khả dụng trong cổng thông tin Azure, tại [Azure Active Directory-> giấy phép-> tất cả sản phẩm](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Người dùng có thể đã có giấy phép khác có các dịch vụ xung đột với những người trong giấy phép mới mà bạn đang cố gắng gán. Ví dụ, nếu người dùng đã bật dịch vụ Exchange Online (gói 1), bạn sẽ không thể gán giấy phép với Exchange Online (gói 2). Vô hiệu hóa một trong các dịch vụ để cho phép gán giấy phép mới. Nếu bạn đang sử dụng các lệnh ghép ngắn Azure Portal hoặc PowerShell, trang **chi tiết vấn đề** liệt kê các dịch vụ cụ thể đang gây ra xung đột.
6. Nếu bạn đang cố gắng loại bỏ giấy phép và không phải là người dùng có thể có các giấy phép khác với các dịch vụ phụ thuộc vào các dịch vụ mà bạn đang cố gắng loại bỏ. Nếu bạn đang sử dụng các lệnh ghép ngắn Azure Portal hoặc PowerShell, thông báo lỗi sẽ liệt kê các dịch vụ cụ thể có phụ thuộc.
7. Nếu bạn muốn hiểu tại sao giấy phép đã được thêm/loại bỏ khỏi một người dùng (ví dụ, những người khác trong tổ chức của bạn có thể đã thực hiện thay đổi), hãy kiểm tra Nhật ký kiểm toán. Đặt bộ lọc vào các **hoạt động giấy phép** để hiển thị tất cả các sửa đổi, bao gồm "diễn viên" đã thực hiện chúng.
8. Nếu bạn đang sử dụng Exchange Online, một số người dùng trong đối tượng thuê của bạn có thể được cấu hình sai với cùng một giá trị địa chỉ proxy. Trong các trường hợp như vậy, bạn có thể thấy thông báo lỗi chung khi thao tác giấy phép không thành công. [Bài viết này](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) chứa thêm thông tin về sự cố này, bao gồm thông tin về [cách kết nối với Exchange Online bằng cách dùng Remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Để xác định người dùng nào trong đối tượng thuê của bạn, chứa cùng một địa chỉ proxy, thực hiện lệnh ghép ngắn Exchange Online này:

Quản

Get-Recipient | trong đó {$ _. EmailAddresses-khớp <user principal name> } | fL name, RecipientType, EmailAddresses





