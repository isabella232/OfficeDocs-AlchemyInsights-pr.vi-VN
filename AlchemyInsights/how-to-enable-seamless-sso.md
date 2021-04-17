---
title: Cách bật SSO liền mạch
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825753"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="bf10c-102">Cách bật SSO liền mạch</span><span class="sxs-lookup"><span data-stu-id="bf10c-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="bf10c-103">Cho phép SSO liền mạch thông qua [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="bf10c-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="bf10c-104">Nếu bạn đang thực hiện một bản cài đặt mới của Azure AD Connect, hãy chọn [đường dẫn cài đặt tùy chỉnh](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="bf10c-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="bf10c-105">Tại trang **đăng nhập người dùng** , hãy chọn tùy chọn **bật đăng nhập đơn** .</span><span class="sxs-lookup"><span data-stu-id="bf10c-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="bf10c-106">Để xác nhận rằng bạn đã bật chính xác SSO đúng cách:</span><span class="sxs-lookup"><span data-stu-id="bf10c-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="bf10c-107">Đăng nhập vào [Trung tâm quản trị Azure Active Directory](https://aad.portal.azure.com) với tư cách là người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="bf10c-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="bf10c-108">Chọn **Azure Active Directory** trong ngăn bên trái.</span><span class="sxs-lookup"><span data-stu-id="bf10c-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="bf10c-109">Xác nhận đăng nhập đơn seamless được **bật**.</span><span class="sxs-lookup"><span data-stu-id="bf10c-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="bf10c-110">Để tìm hiểu thêm, hãy xem [Azure Active Directory liền mạch Single đăng nhập: bắt đầu nhanh](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="bf10c-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  