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
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="fee79-102">Vấn đề với Azure MFA</span><span class="sxs-lookup"><span data-stu-id="fee79-102">Issues with Azure MFA</span></span>
<span data-ttu-id="fee79-103">Có một vài điều cần kiểm tra xem người dùng không thể đăng nhập bằng cách sử dụng xác thực đa yếu tố (MFA)</span><span class="sxs-lookup"><span data-stu-id="fee79-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="fee79-104">Người dùng bị ảnh hưởng có thể bị chặn trong cổng Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fee79-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="fee79-105">Nếu đó là trường hợp, các nỗ lực xác thực cho người dùng cụ thể đó sẽ tự động bị từ chối.</span><span class="sxs-lookup"><span data-stu-id="fee79-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="fee79-106">Vui lòng làm theo các bước trong bài viết này để bỏ chặn chúng.</span><span class="sxs-lookup"><span data-stu-id="fee79-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="fee79-107">Nếu bỏ chặn người dùng không giúp đỡ hoặc người dùng không bị chặn, bạn có thể thử đặt lại MFA cho người dùng và họ sẽ đi qua quá trình đăng ký một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="fee79-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="fee79-108">Vui lòng làm theo các bước trong bài viết này.</span><span class="sxs-lookup"><span data-stu-id="fee79-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="fee79-109">Nếu đây là lần đầu tiên bạn kích hoạt MFA và người dùng của bạn không thể đăng nhập vào các trình duyệt không phải là các khách hàng như Outlook, Skype, vv, có lẽ ADAL (Active Directory xác thực thư viện) không được kích hoạt trên O365 đăng ký của bạn.</span><span class="sxs-lookup"><span data-stu-id="fee79-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="fee79-110">Trong trường hợp này, bạn sẽ cần phải kết nối với Exchange Online PowerShell và chạy lệnh này:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="fee79-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>