---
title: Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) dựa trên mật khẩu
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714910"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="65887-102">Khắc phục sự cố các vấn đề đăng nhập đơn (SSO) dựa trên mật khẩu</span><span class="sxs-lookup"><span data-stu-id="65887-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="65887-103">Để tìm hiểu các nguyên tắc cơ bản của SSO dựa trên mật khẩu, hãy xem [xác thực dựa trên mật khẩu với Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="65887-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="65887-104">**Đặt cấu hình SSO dựa trên mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="65887-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="65887-105">[Đặt cấu hình đăng nhập đơn dựa trên mật khẩu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) -bài viết này đi sâu vào chi tiết hơn về tùy chọn SSO dựa trên mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="65887-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="65887-106">Nếu ứng dụng bạn đang thêm yêu cầu cấu hình tùy chỉnh và bạn cần sử dụng SSO dựa trên mật khẩu, thì bài viết này là dành cho bạn.</span><span class="sxs-lookup"><span data-stu-id="65887-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="65887-107">[Đặt cấu hình đăng nhập đơn dựa trên mật khẩu cho ứng dụng Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) -proxy hỗ trợ một số chế độ đăng nhập đơn.</span><span class="sxs-lookup"><span data-stu-id="65887-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="65887-108">Đăng nhập dựa trên mật khẩu được dành cho các ứng dụng sử dụng kết hợp tên người dùng/mật khẩu để xác thực.</span><span class="sxs-lookup"><span data-stu-id="65887-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="65887-109">Khi bạn cấu hình đăng ký dựa trên mật khẩu cho ứng dụng của bạn, người dùng của bạn phải đăng nhập vào ứng dụng tại cơ sở một lần.</span><span class="sxs-lookup"><span data-stu-id="65887-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="65887-110">Sau đó, Azure Active Directory lưu trữ thông tin đăng nhập và tự động cung cấp cho ứng dụng khi người dùng của bạn truy nhập từ xa.</span><span class="sxs-lookup"><span data-stu-id="65887-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="65887-111">Bạn nên đã được phát hành và thử nghiệm ứng dụng của bạn với proxy ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="65887-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="65887-112">Nếu không, hãy làm theo các bước trong phát hành các [ứng dụng bằng cách sử dụng ứng dụng AZURE AD proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) sau đó tiếp tục cấu hình của bạn trong SSO dựa trên mật khẩu cho các ứng dụng trên Prem.</span><span class="sxs-lookup"><span data-stu-id="65887-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="65887-113">Để khắc phục sự cố SSO dựa trên mật khẩu, hãy xem [khắc phục sự cố đăng nhập đơn trên mật khẩu trong AZURE AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="65887-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
