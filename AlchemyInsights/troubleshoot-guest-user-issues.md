---
title: Khắc phục sự cố người dùng khách
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901595"
---
# <a name="troubleshoot-guest-user-issues"></a>Khắc phục sự cố người dùng khách

1. Để được hướng dẫn về việc quản lý quyền truy nhập của khách vào các ứng dụng, hãy xem mục [quản lý quyền truy nhập khách với AZURE AD Access](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. [Thêm người dùng khách vào danh bạ của bạn trong cổng thông tin Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): trong bắt đầu nhanh này, bạn sẽ thêm một người dùng khách mới vào thư mục Azure AD của bạn qua cổng Azure, gửi lời mời và xem quy trình trả lời thư mời của người dùng khách trông như thế nào.
1. [Thêm người dùng khách với PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): trong bắt đầu nhanh này, bạn sẽ sử dụng lệnh New-AzureADMSInvitation để thêm một người dùng khách vào đối tượng Azure của bạn.
1. Để tìm hiểu cách gán người dùng và nhóm, đến các ứng dụng doanh nghiệp trong Azure Active Directory (Azure AD), từ trong cổng thông tin Azure hoặc bằng cách sử dụng PowerShell, hãy xem [quản lý việc gán người dùng cho một ứng dụng trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) cộng tác B2B làm việc với hầu hết các ứng dụng tích hợp với Azure AD. Trong [bài viết](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)này, chúng tôi hướng dẫn để cấu hình một số ứng dụng Saas phổ biến để sử dụng với AZURE AD B2B.
1. Với tư cách là một tổ chức sử dụng Azure Active Directory (Azure AD) các khả năng cộng tác B2B để mời người dùng khách từ các tổ chức đối tác đến Azure AD của bạn, bạn có thể cung cấp những người dùng B2B này quyền truy nhập vào các ứng dụng tại cơ sở. Những ứng dụng tại cơ sở này có thể sử dụng xác thực dựa trên SAML hoặc xác thực Windows tích hợp (IWA) với ủy quyền Kerberos ràng buộc (KCD). Để biết thêm thông tin, hãy xem [cấp cho người dùng B2B trong AZURE AD Access vào các ứng dụng tại chỗ của bạn](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Tìm hiểu cách [cấp quyền truy nhập tài khoản đối tác được quản lý cục bộ vào tài nguyên điện toán đám mây bằng cách sử dụng AZURE AD B2B cộng tác](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).