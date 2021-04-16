---
title: Các vấn đề với MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810506"
---
# <a name="issues-with-azure-mfa"></a>Các vấn đề với Azure MFA
Có một vài điều cần kiểm tra xem liệu người dùng không thể đăng nhập bằng xác thực đa yếu tố (MFA)

1. Người dùng bị ảnh hưởng có thể bị chặn trong cổng thông tin Azure Active Directory. Nếu đó là trường hợp, các nỗ lực xác thực đối với người dùng cụ thể này sẽ bị từ chối tự động. [Vui lòng làm theo các bước trong bài viết này để bỏ chặn chúng.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Nếu bỏ chặn người dùng không trợ giúp hoặc người dùng không bị chặn, bạn có thể tìm cách đặt lại MFA cho người dùng và họ sẽ đi qua quy trình đăng ký lần nữa. [Vui lòng làm theo các bước trong bài viết này.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Nếu đây là lần đầu tiên bạn bật MFA và người dùng của bạn không thể đăng nhập vào các máy khách không phải trình duyệt chẳng hạn như Outlook, Skype, v.v., có lẽ là ADAL (Active Directory xác thực thư viện) không được kích hoạt trên đăng ký O365 của bạn. Trong trường hợp này, bạn sẽ cần kết nối với Exchange Online PowerShell và chạy lệnh ghép ngắn này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*