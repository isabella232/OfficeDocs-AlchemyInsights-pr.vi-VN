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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="e9011-102">Các vấn đề với Azure MFA</span><span class="sxs-lookup"><span data-stu-id="e9011-102">Issues with Azure MFA</span></span>
<span data-ttu-id="e9011-103">Có một vài điều cần kiểm tra xem liệu người dùng không thể đăng nhập bằng xác thực đa yếu tố (MFA)</span><span class="sxs-lookup"><span data-stu-id="e9011-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="e9011-104">Người dùng bị ảnh hưởng có thể bị chặn trong cổng thông tin Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e9011-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="e9011-105">Nếu đó là trường hợp, các nỗ lực xác thực đối với người dùng cụ thể này sẽ bị từ chối tự động.</span><span class="sxs-lookup"><span data-stu-id="e9011-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="e9011-106">Vui lòng làm theo các bước trong bài viết này để bỏ chặn chúng.</span><span class="sxs-lookup"><span data-stu-id="e9011-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="e9011-107">Nếu bỏ chặn người dùng không trợ giúp hoặc người dùng không bị chặn, bạn có thể tìm cách đặt lại MFA cho người dùng và họ sẽ đi qua quy trình đăng ký lần nữa.</span><span class="sxs-lookup"><span data-stu-id="e9011-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="e9011-108">Vui lòng làm theo các bước trong bài viết này.</span><span class="sxs-lookup"><span data-stu-id="e9011-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="e9011-109">Nếu đây là lần đầu tiên bạn bật MFA và người dùng của bạn không thể đăng nhập vào các máy khách không phải trình duyệt chẳng hạn như Outlook, Skype, v.v., có lẽ là ADAL (Active Directory xác thực thư viện) không được kích hoạt trên đăng ký O365 của bạn.</span><span class="sxs-lookup"><span data-stu-id="e9011-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="e9011-110">Trong trường hợp này, bạn sẽ cần kết nối với Exchange Online PowerShell và chạy lệnh ghép ngắn này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="e9011-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>