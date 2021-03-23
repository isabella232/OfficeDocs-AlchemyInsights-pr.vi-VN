---
title: Làm việc với thư viện xác thực
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036863"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="5136f-102">Làm việc với thư viện xác thực</span><span class="sxs-lookup"><span data-stu-id="5136f-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="5136f-103">Để giải quyết sự cố về thư viện xác thực của Microsoft (MSAL), hãy thực hiện các bước được đề xuất sau đây:</span><span class="sxs-lookup"><span data-stu-id="5136f-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="5136f-104">**Làm việc với MSAL**: [Thư viện xác thực nền tảng căn cước Microsoft](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) -bài viết này hiển thị hỗ trợ thư viện xác thực Microsoft cho một số loại ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="5136f-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="5136f-105">Nó bao gồm các nối kết đến mã nguồn thư viện; nơi nhận gói cho dự án ứng dụng của bạn; và liệu thư viện hỗ trợ đăng nhập của người dùng (xác thực), truy nhập vào các API web được bảo vệ (ủy quyền) hoặc cả hai.</span><span class="sxs-lookup"><span data-stu-id="5136f-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="5136f-106">**Khắc phục sự cố xác thực**: hàm msal hỗ trợ một số dòng xác thực để sử dụng trong các kịch bản ứng dụng khác nhau.</span><span class="sxs-lookup"><span data-stu-id="5136f-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="5136f-107">Tùy thuộc vào cách thức ứng dụng khách của bạn được xây dựng, thì MSAL có thể sử dụng một hoặc nhiều dòng xác thực được hỗ trợ bởi nền tảng định danh Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5136f-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="5136f-108">Những dòng này có thể tạo ra một số loại thẻ và mã ủy quyền và yêu cầu các thẻ khác nhau để làm cho chúng hoạt động.</span><span class="sxs-lookup"><span data-stu-id="5136f-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="5136f-109">**Thẻ Access**: [thẻ truy nhập Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -tìm hiểu cách API của bạn có thể xác thực và sử dụng các tuyên bố bên trong mã thông báo Access.</span><span class="sxs-lookup"><span data-stu-id="5136f-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="5136f-110">Tất cả tài liệu trong bài viết này, ngoại trừ khi ghi chú, chỉ áp dụng cho các thẻ được phát hành cho các API mà bạn đã đăng ký.</span><span class="sxs-lookup"><span data-stu-id="5136f-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="5136f-111">Nó không áp dụng cho các thẻ được phát hành cho các API Microsoft thuộc sở hữu, cũng không thể dùng thẻ này để xác thực cách Microsoft Identity Platform sẽ phát hành thẻ cho API bạn tạo ra.</span><span class="sxs-lookup"><span data-stu-id="5136f-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="5136f-112">**Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="5136f-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="5136f-113">**Bắt đầu từ ngày 30 tháng 6, 2020,** chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Adal và Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="5136f-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="5136f-114">Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.</span><span class="sxs-lookup"><span data-stu-id="5136f-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="5136f-115">**Bắt đầu từ ngày 30 tháng 6, 2022,** chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.</span><span class="sxs-lookup"><span data-stu-id="5136f-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="5136f-116">Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không *nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào*.</span><span class="sxs-lookup"><span data-stu-id="5136f-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="5136f-117">Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="5136f-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="5136f-118">**Di chuyển ADAL**</span><span class="sxs-lookup"><span data-stu-id="5136f-118">**ADAL Migration**</span></span>

- <span data-ttu-id="5136f-119">Chúng tôi khuyên bạn nên cập nhật lên MSAL, trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.</span><span class="sxs-lookup"><span data-stu-id="5136f-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="5136f-120">Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ bảo mật liên tục và cải thiện tính năng của MSAL.</span><span class="sxs-lookup"><span data-stu-id="5136f-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="5136f-121">[Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="5136f-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="5136f-122">[Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="5136f-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="5136f-123">Nếu sau khi đọc hướng dẫn dành cho nền tảng ứng dụng của bạn, bạn có thêm câu hỏi, bạn có thể đăng lên [Microsoft hỏi&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) bằng thẻ [Azure-AD-Adal-deprecation] hoặc mở một vấn đề trong kho lưu trữ của thư viện.</span><span class="sxs-lookup"><span data-stu-id="5136f-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="5136f-124">Xem phần [ngôn ngữ và khung](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) của bài viết **tổng quan về msal** cho các nối kết đến repo của mỗi thư viện.</span><span class="sxs-lookup"><span data-stu-id="5136f-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="5136f-125">**Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL**, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn.</span><span class="sxs-lookup"><span data-stu-id="5136f-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="5136f-126">Nếu áp dụng, hãy tiếp cận với bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="5136f-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="5136f-127">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="5136f-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







