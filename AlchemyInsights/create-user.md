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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747032"
---
# <a name="create-user"></a>Tạo người dùng

**THÔNG**

- [Deprecation của WebView hỗ trợ đăng nhập từ Google bắt đầu từ 4 tháng 1, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Kiểm tra xem các ứng dụng của bạn có thể bị ảnh hưởng bằng cách làm theo [hướng dẫn của Google](https://go.microsoft.com/fwlink/?linkid=2157323) khi kiểm tra tính tương thích.
- Hãy đảm bảo bạn sử dụng trình duyệt hệ thống WebView hoặc hệ thống khi đăng nhập vào người dùng của bạn với tài khoản Google dành cho người dùng. Để biết thêm thông tin, hãy xem các [vấn đề đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Tôi không thể tạo người dùng mới trong thư mục Azure AD của tôi**

1. Đảm bảo rằng bạn được ủy quyền để tạo một người dùng tiêu chuẩn mới. Chỉ người quản trị toàn cầu hoặc vai trò người quản trị người dùng trong Azure Active Directory (AD) có thể tạo một người dùng chuẩn mới. Nếu bạn không ở trong một trong những vai trò này, hãy yêu cầu người quản trị thêm bạn vào một trong những vai trò này hoặc để tạo tài khoản người dùng mới cho bạn.
1. Đảm bảo rằng tên người dùng đang ở trong một tên miền được xác minh trong Azure AD của bạn. Nếu bạn không có bất kỳ tên miền riêng nào được xác minh trong Azure AD, bạn có thể sử dụng tên miền Azure AD ban đầu của bạn, kết thúc bằng *. onmicrosoft.com.
1. Đảm bảo rằng tên người dùng đang ở trong một tên miền không được liên kết với Azure AD từ quảng cáo tại cơ sở của bạn. Người dùng không thể được thêm vào điện toán đám mây có tên miền được liên kết từ tại cơ sở.
1. Đảm bảo rằng không có người dùng hoặc liên hệ nào khác đã có tên người dùng mà bạn muốn gán cho người dùng mới. Tên người dùng phải là duy nhất trên Azure AD.
1. Xem các [vai trò và người quản trị AZURE AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) cho Azure AD của bạn.
1. Xem [tên miền](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) cho Azure AD của bạn.
1. Xem lại [Nhật ký kiểm](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) tra để xem thông tin chi tiết hơn về một người dùng đã tạo hoặc đã xóa gần đây như những người thực hiện hành động và khi nào.
1. Để biết thêm thông tin về cách thêm người dùng mới, hãy xem [sử dụng cổng thông tin Azure để tạo người dùng mới trong AZURE AD của bạn](/azure/active-directory/active-directory-users-create-azure-portal).
1. Các [vai trò quản trị AZURE AD](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): quyền của vai trò người quản trị trong Azure Active Directory
1. Bạn cũng có thể [sử dụng AZURE AD PowerShell để tạo người dùng mới](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
