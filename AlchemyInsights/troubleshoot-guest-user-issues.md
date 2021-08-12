---
title: Khắc phục sự cố về người dùng khách
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
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939401"
---
# <a name="troubleshoot-guest-user-issues"></a>Khắc phục sự cố về người dùng khách

1. Để biết hướng dẫn về việc quản lý quyền truy nhập của khách vào các ứng dụng, hãy xem mục [Quản lý quyền truy nhập khách với đánh giá quyền truy nhập Azure AD.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. Thêm người dùng khách vào thư mục của bạn trong cổng thông tin [Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)Trong hướng dẫn nhanh này, bạn sẽ thêm một người dùng khách mới vào thư mục Azure AD thông qua cổng thông tin Azure, gửi lời mời và xem giao diện quy trình quy đổi lời mời của người dùng khách.
1. [Thêm người dùng khách với PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)Trong bắt đầu nhanh này, bạn sẽ sử dụng lệnh New-AzureADMSInvitation để thêm một người dùng khách vào đối tượng thuê Azure của mình.
1. Để tìm hiểu cách gán người dùng và nhóm cho các ứng dụng doanh nghiệp trong Azure Active Directory (Azure AD), hoặc từ bên trong cổng thông tin Azure hoặc bằng cách sử dụng PowerShell, hãy xem mục Quản lý việc gán người dùng cho một ứng dụng [trong Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory tác B2B (Azure AD) hoạt động với hầu hết các ứng dụng tích hợp với Azure AD. Trong bài [viết này,](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)chúng tôi sẽ hướng dẫn cách đặt cấu hình một số ứng dụng SaaS phổ biến để sử dụng với Azure AD B2B.
1. Với tư cách là một tổ chức sử dụng các chức năng cộng tác B2B của Azure Active Directory (Azure AD) để mời người dùng khách từ tổ chức đối tác đến Azure AD của bạn, giờ đây bạn có thể cung cấp quyền truy nhập cho những người dùng B2B này vào các ứng dụng tại chỗ. Các ứng dụng tại chỗ này có thể sử dụng xác thực dựa trên SAML hoặc Xác thực Windows Tích hợp (IWA) với ủy quyền ràng buộc của Kerberos (KCD). Để biết thêm thông tin, [hãy xem mục Cấp cho người dùng B2B quyền truy nhập Azure AD vào các ứng dụng tại chỗ của bạn.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Tìm hiểu cách cấp quyền [truy nhập tài khoản đối tác được quản lý cục bộ vào các tài nguyên đám mây bằng cách sử dụng cộng tác Azure AD B2B.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)