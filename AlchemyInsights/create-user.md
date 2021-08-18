---
title: Tạo người dùng
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: d86b2dd6d7915f0698cf950cd57f1065cde22219284edbbc0e64f3a5e69ff252
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896737"
---
# <a name="create-user"></a>Tạo người dùng

**THÔNG BÁO:**

- Không còn hỗ trợ đăng nhập WebView từ Google kể từ ngày 4 tháng [1 năm 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Kiểm tra xem các ứng dụng của bạn có thể bị ảnh hưởng bởi việc làm theo [hướng dẫn của Google về](https://go.microsoft.com/fwlink/?linkid=2157323) việc kiểm tra tính tương thích hay không.
- Đảm bảo bạn sử dụng dạng xem web hệ thống hoặc trình duyệt hệ thống khi đăng nhập người dùng bằng tài khoản Google dành cho người tiêu dùng. Để biết thêm thông tin, [hãy xem mục Sự cố đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Tôi không thể tạo người dùng mới trong thư mục Azure AD của mình**

1. Đảm bảo rằng bạn được phép tạo người dùng tiêu chuẩn mới. Chỉ người quản trị Toàn cầu hoặc vai trò người quản trị Người dùng trong Azure Active Directory (AD) mới có thể tạo một người dùng chuẩn mới. Nếu bạn không ở trong một trong những vai trò này, hãy yêu cầu người quản trị thêm bạn vào một trong những vai trò này hoặc tạo tài khoản người dùng mới cho bạn.
1. Đảm bảo rằng tên người dùng nằm trong miền được xác minh trong Azure AD của bạn. Nếu bạn không có bất kỳ tên miền riêng đã xác minh nào trong Azure AD, bạn có thể sử dụng miền ban đầu Azure AD kết thúc bằng *.onmicrosoft.com.
1. Đảm bảo rằng tên người dùng nằm trong một miền không được liên kết với Azure AD từ AD tại chỗ của bạn. Không thể thêm người dùng vào đám mây với các tên miền được liên kết từ tại chỗ.
1. Đảm bảo rằng không có người dùng hoặc liên hệ nào khác đã có tên người dùng mà bạn muốn gán cho người dùng mới. Tên người dùng phải là duy nhất trong Azure AD.
1. Hãy [xem mục Vai trò và người quản trị Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) cho Azure AD của bạn.
1. Xem các [tên miền cho](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD của bạn.
1. Xem [lại Nhật ký kiểm tra](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) để xem thông tin chi tiết hơn về người dùng được tạo hoặc xóa gần đây như người đã thực hiện hành động và thời điểm thực hiện hành động.
1. Để biết thêm thông tin về cách thêm người dùng mới, hãy [xem mục Sử dụng cổng thông tin Azure để tạo người dùng mới trong Azure AD của bạn.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Vai trò quản trị Azure AD:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Quyền vai trò người quản trị trong Azure Active Directory
1. Bạn cũng có [thể sử dụng Azure AD PowerShell để tạo người dùng mới.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
