---
title: Sự cố với MFA
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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098624"
---
# <a name="issues-with-azure-mfa"></a>Sự cố với Azure MFA
Có một số điều cần kiểm tra xem người dùng không thể đăng nhập bằng xác thực đa yếu tố (MFA)

1. Người dùng bị ảnh hưởng có thể bị chặn trong Azure Active Directory Portal. Nếu như vậy, nỗ lực xác thực của người dùng cụ thể đó sẽ tự động bị từ chối. [Vui lòng làm theo các bước trong bài viết này để bỏ chặn chúng.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Nếu việc bỏ chặn người dùng không giúp ích hoặc người dùng không bị chặn, bạn có thể tìm cách đặt lại MFA cho người dùng và họ sẽ thực hiện lại quy trình đăng ký. [Vui lòng làm theo các bước trong bài viết này.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Nếu đây là lần đầu bạn bật MFA và người dùng của bạn không thể đăng nhập vào các máy khách không phải trình duyệt, chẳng hạn như Outlook, Skype, v.v. có thể ADAL (Thư viện Xác thực Active Directory) không được bật trên thuê bao O365 của bạn. Trong trường hợp này, bạn sẽ cần kết nối với Exchange Online Powershell, rồi chạy lệnh ghép ngắn này: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*