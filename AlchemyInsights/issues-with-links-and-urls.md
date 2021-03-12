---
title: Các vấn đề với liên kết và URL
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: f682afc2006957a83d02973d28e2a07ee63ac888
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707904"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="fb970-102">Các vấn đề với liên kết và URL</span><span class="sxs-lookup"><span data-stu-id="fb970-102">Issues with links and URLs</span></span>

<span data-ttu-id="fb970-103">URL chuyển hướng/trả lời (cả hai biểu thức đều có thể hoán đổi) là các URL được dùng bởi nền tảng định danh Microsoft để trả về các thẻ yêu cầu ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="fb970-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="fb970-104">Để biết thông tin về các URL này, hãy xem các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="fb970-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="fb970-105">Các [dòng xác thực và kịch bản ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) -thông tin về việc chuyển hướng đến URIs trong trang **đăng ký ứng dụng** cho từng tình huống.</span><span class="sxs-lookup"><span data-stu-id="fb970-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="fb970-106">Các hạn chế và giới hạn URL chuyển hướng URI/trả lời</span><span class="sxs-lookup"><span data-stu-id="fb970-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="fb970-107">**Tôi không biết làm thế nào để đăng ký URI chuyển hướng bên phải/trả lời URL cho ứng dụng của tôi**</span><span class="sxs-lookup"><span data-stu-id="fb970-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="fb970-108">Khi bạn đăng nhập bằng ứng dụng bạn đang phát triển, nếu hộp thoại đăng nhập Hiển thị **AADSTS50011: URL trả lời được xác định trong yêu cầu không khớp với URL trả lời được <your app ID> cấu hình cho ứng dụng**, bạn sẽ cần phải thêm vào đăng ký ứng dụng của mình, URI chuyển hướng mà mã của bạn được sử dụng trong yêu cầu mã thông báo đến nền tảng Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="fb970-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="fb970-109">Để thêm URL trả lời, hãy đi đến tab **xác thực** trong trang **đăng ký ứng dụng** của bạn trong cổng thông tin Azure và thêm một mục nhập trong phần **chuyển hướng URIs** .</span><span class="sxs-lookup"><span data-stu-id="fb970-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="fb970-110">Giá trị bạn cần nhập tùy thuộc vào loại ứng dụng mà bạn đang xây dựng, như được mô tả dưới đây:</span><span class="sxs-lookup"><span data-stu-id="fb970-110">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="fb970-111">Đối với các ứng dụng trang đơn và ứng dụng web, URL trả lời là một URL trong ứng dụng của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb970-111">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="fb970-112">Xem [đăng ký ứng dụng trang đơn](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) hoặc [đăng ký ứng dụng Web App bằng cách dùng Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="fb970-112">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="fb970-113">Đối với các ứng dụng trên máy tính, giá trị mà bạn cần chọn tùy thuộc vào:</span><span class="sxs-lookup"><span data-stu-id="fb970-113">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="fb970-114">nền tảng (MacOS khác với Windows hoặc Linux)</span><span class="sxs-lookup"><span data-stu-id="fb970-114">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="fb970-115">cách bạn thu thập mã thông báo (tương tác, với dòng mã thiết bị, với xác thực Windows tích hợp [IWA] hoặc với tên người dùng/mật khẩu).</span><span class="sxs-lookup"><span data-stu-id="fb970-115">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="fb970-116">Để biết chi tiết, hãy xem [ứng dụng trên máy tính-đăng ký ứng dụng-URi chuyển hướng](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="fb970-116">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="fb970-117">Đối với các ứng dụng dành cho thiết bị di động, URI chuyển hướng phụ thuộc vào:</span><span class="sxs-lookup"><span data-stu-id="fb970-117">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="fb970-118">nền tảng (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="fb970-118">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="fb970-119">thông tin được sử dụng để xây dựng ứng dụng của bạn, chẳng hạn như ID gói trong iOS và tên gói và chữ ký băm trên thiết bị đăng ký ứng dụng Azure Portal sẽ giúp bạn.</span><span class="sxs-lookup"><span data-stu-id="fb970-119">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="fb970-120">Để biết chi tiết, hãy xem [cấu hình nền tảng và chuyển hướng URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="fb970-120">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="fb970-121">Các API web và một số cách thức để có được thẻ (IWA và tên người dùng/mật khẩu) không yêu cầu một URI chuyển hướng.</span><span class="sxs-lookup"><span data-stu-id="fb970-121">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="fb970-122">**Tôi đã triển khai ứng dụng web của mình và khi tôi kiểm tra ứng dụng đã triển khai, tôi nhận được thông báo không khớp với URL trả lời**</span><span class="sxs-lookup"><span data-stu-id="fb970-122">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="fb970-123">Thêm chuyển hướng URIs cho tất cả các vị trí mà tại đó bạn đang triển khai ứng dụng web của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb970-123">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="fb970-124">Để biết thêm thông tin, hãy xem mục [đăng ký ứng dụng Web App bằng Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span><span class="sxs-lookup"><span data-stu-id="fb970-124">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="fb970-125">Thêm URI chuyển hướng cho một vị trí ngay sau khi bạn đã triển khai ứng dụng tại vị trí đó.</span><span class="sxs-lookup"><span data-stu-id="fb970-125">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="fb970-126">**Tôi không thể đăng ký đủ URL trả lời**</span><span class="sxs-lookup"><span data-stu-id="fb970-126">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="fb970-127">Bạn là một ISV và có một hoặc nhiều chuyển hướng URIs cho mọi khách hàng của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb970-127">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="fb970-128">Bạn muốn di chuyển từ ADAL/Azure AD v 1.0 sang MSAL/nền tảng định danh Microsoft và bạn nhấn vào [số lượng chuyển hướng tối đa của URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span><span class="sxs-lookup"><span data-stu-id="fb970-128">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="fb970-129">Để giải quyết vấn đề này, hãy [Thêm chuyển hướng URIs vào hiệu trưởng dịch vụ](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) tương ứng với từng khách hàng của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb970-129">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
