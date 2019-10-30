---
title: Các vấn đề về MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768859"
---
# <a name="issues-with-azure-mfa"></a>Vấn đề với Azure MFA
Có một vài điều cần kiểm tra xem người dùng không thể đăng nhập bằng cách sử dụng xác thực đa yếu tố (MFA)

1. Người dùng bị ảnh hưởng có thể bị chặn trong cổng Azure Active Directory. Nếu đó là trường hợp, các nỗ lực xác thực cho người dùng cụ thể đó sẽ tự động bị từ chối. [Vui lòng làm theo các bước trong bài viết này để bỏ chặn chúng.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Nếu bỏ chặn người dùng không giúp đỡ hoặc người dùng không bị chặn, bạn có thể thử đặt lại MFA cho người dùng và họ sẽ đi qua quá trình đăng ký một lần nữa. [Vui lòng làm theo các bước trong bài viết này.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Nếu đây là lần đầu tiên bạn kích hoạt MFA và người dùng của bạn không thể đăng nhập vào các trình duyệt không phải là các khách hàng như Outlook, Skype, vv, có lẽ ADAL (Active Directory xác thực thư viện) không được kích hoạt trên O365 đăng ký của bạn. Trong trường hợp này, bạn sẽ cần phải kết nối với Exchange Online PowerShell và chạy lệnh này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*