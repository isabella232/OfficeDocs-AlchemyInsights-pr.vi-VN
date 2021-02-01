---
title: Các vấn đề với thư viện xác thực
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063704"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="4948a-102">Các vấn đề với thư viện xác thực</span><span class="sxs-lookup"><span data-stu-id="4948a-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="4948a-103">[Thư viện xác thực nền tảng Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) liệt kê các thư viện ứng dụng và máy khách tương thích của Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4948a-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="4948a-104">Thư viện xác thực Microsoft (MSAL) hỗ trợ một số [dòng xác thực](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) để sử dụng trong các kịch bản ứng dụng khác nhau.</span><span class="sxs-lookup"><span data-stu-id="4948a-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="4948a-105">Để xác thực và lấy thẻ, bạn khởi tạo một ứng dụng khách công cộng hoặc bảo mật mới trong mã của bạn.</span><span class="sxs-lookup"><span data-stu-id="4948a-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="4948a-106">Bạn có thể thiết lập một số tùy chọn cấu hình khi khởi tạo ứng dụng khách trong thư viện xác thực Microsoft (MSAL).</span><span class="sxs-lookup"><span data-stu-id="4948a-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="4948a-107">Để tìm hiểu thêm, hãy xem [tùy chọn cấu hình ứng dụng](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="4948a-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="4948a-108">**Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and Azure AD graph API (đồ họa Bad)**</span><span class="sxs-lookup"><span data-stu-id="4948a-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="4948a-109">**Bắt đầu từ ngày 30 tháng 6, 2020**, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Adal và Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="4948a-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="4948a-110">Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.</span><span class="sxs-lookup"><span data-stu-id="4948a-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="4948a-111">**Bắt đầu từ ngày 30 tháng 6, 2022**, chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.</span><span class="sxs-lookup"><span data-stu-id="4948a-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="4948a-112">Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không *nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào*.</span><span class="sxs-lookup"><span data-stu-id="4948a-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="4948a-113">Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="4948a-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="4948a-114">**Di chuyển ADAL**</span><span class="sxs-lookup"><span data-stu-id="4948a-114">**ADAL Migration**</span></span>

<span data-ttu-id="4948a-115">Chúng tôi khuyên bạn nên cập nhật lên [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.</span><span class="sxs-lookup"><span data-stu-id="4948a-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="4948a-116">Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển các ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ các cải thiện về bảo mật và tính năng của MSAL.</span><span class="sxs-lookup"><span data-stu-id="4948a-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="4948a-117">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="4948a-117">For more information, see:</span></span>

1. [<span data-ttu-id="4948a-118">Đọc các câu hỏi thường gặp về ADAL</span><span class="sxs-lookup"><span data-stu-id="4948a-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="4948a-119">Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng</span><span class="sxs-lookup"><span data-stu-id="4948a-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="4948a-120">Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào.</span><span class="sxs-lookup"><span data-stu-id="4948a-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="4948a-121">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="4948a-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="4948a-122">**Di chuyển đồ thị trong Bad**</span><span class="sxs-lookup"><span data-stu-id="4948a-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="4948a-123">Đối với các ứng dụng đang sử dụng đồ thị Azure AD, hãy làm theo hướng dẫn của chúng tôi để [di chuyển các ứng dụng đồ thị AZURE AD sang Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="4948a-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="4948a-124">Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="4948a-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="4948a-125">Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad.</span><span class="sxs-lookup"><span data-stu-id="4948a-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="4948a-126">Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào.</span><span class="sxs-lookup"><span data-stu-id="4948a-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="4948a-127">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả việc sử dụng đồ thị trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="4948a-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="4948a-128">Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận.</span><span class="sxs-lookup"><span data-stu-id="4948a-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="4948a-129">[Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="4948a-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="4948a-130">Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.</span><span class="sxs-lookup"><span data-stu-id="4948a-130">It also provides guidance about how to use the permissions.</span></span>
