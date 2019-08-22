---
title: Vấn đề với MFA
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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545208"
---
# <a name="issues-with-mfa"></a>Vấn đề với MFA
Có một vài điều để kiểm tra nếu người dùng không thể đăng nhập bằng cách sử dụng nhiều yếu tố xác thực (MFA)

1. Người dùng bị ảnh hưởng có thể bị chặn trong Azure Active Directory cổng. Nếu trường hợp đó xảy ra, xác thực nỗ lực cho rằng người dùng cụ thể sẽ được tự động bị từ chối. [Xin vui lòng làm theo các bước trong bài viết này để bỏ chặn họ.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Nếu bỏ chặn người dùng đã không giúp đỡ hoặc không chặn người dùng bạn có thể thử đặt lại MFA cho người dùng và họ sẽ đi qua quá trình ghi danh một lần nữa. [Xin vui lòng làm theo các bước trong bài viết này.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Nếu đây là lần đầu tiên bạn kích hoạt MFA và người dùng của bạn là không thể đăng nhập vào trình duyệt không khách hàng chẳng hạn như Outlook, Skype, vv, có lẽ ADAL (Active Directory xác thực thư viện) không được kích hoạt trên đăng ký của bạn O365. Trong trường hợp này bạn sẽ cần để kết nối với Exchange Online Powershell và chạy lệnh ghép ngắn này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*