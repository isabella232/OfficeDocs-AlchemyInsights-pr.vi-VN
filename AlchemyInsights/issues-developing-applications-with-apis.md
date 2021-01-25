---
title: Các vấn đề đang phát triển các ứng dụng với API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975023"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="fe6f1-102">Các vấn đề đang phát triển các ứng dụng với API</span><span class="sxs-lookup"><span data-stu-id="fe6f1-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="fe6f1-103">Để bắt đầu sử dụng API của Azure Active Directory graph, hãy xem [hướng dẫn bắt đầu của AZURE AD graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , hoặc xem [tài liệu tham khảo của AZURE AD graph API tương tác](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="fe6f1-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="fe6f1-104">**Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and Azure AD graph API (đồ họa Bad)**</span><span class="sxs-lookup"><span data-stu-id="fe6f1-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="fe6f1-105">**Bắt đầu từ ngày 30 tháng 6, 2020**, chúng tôi sẽ không còn thêm bất kỳ tính năng mới nào vào Adal và Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="fe6f1-106">Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="fe6f1-107">**Bắt đầu từ ngày 30 tháng 6, 2022**, chúng tôi sẽ kết thúc hỗ trợ cho Adal và Azure AD graph và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="fe6f1-108">Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="fe6f1-109">Các ứng dụng bằng cách sử dụng đồ thị Azure AD sau khi thời gian này không còn nhận được phản hồi từ điểm cuối Azure AD graph.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="fe6f1-110">**Di chuyển ADAL**</span><span class="sxs-lookup"><span data-stu-id="fe6f1-110">**ADAL Migration**</span></span>

<span data-ttu-id="fe6f1-111">Chúng tôi khuyên bạn nên cập nhật lên [Thư viện xác thực Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="fe6f1-112">Nếu bạn đang sử dụng ứng dụng Microsoft, hãy biết rằng Microsoft đang trong quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối hỗ trợ, đảm bảo rằng họ sẽ lợi ích từ bảo mật liên tục và cải thiện tính năng của MSAL.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="fe6f1-113">[Đọc các câu hỏi thường gặp về ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="fe6f1-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="fe6f1-114">[Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="fe6f1-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="fe6f1-115">Nếu bạn cần trợ giúp về các ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="fe6f1-116">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="fe6f1-117">**Di chuyển đồ thị trong Bad**</span><span class="sxs-lookup"><span data-stu-id="fe6f1-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="fe6f1-118">Đối với các ứng dụng đang sử dụng đồ thị Azure AD, hãy làm theo hướng dẫn của chúng tôi để di chuyển các [ứng dụng đồ thị AZURE AD sang Microsoft graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="fe6f1-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="fe6f1-119">[Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="fe6f1-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="fe6f1-120">Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="fe6f1-121">Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp dịch vụ ISVs hoặc ứng dụng nào.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="fe6f1-122">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả việc sử dụng đồ thị trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="fe6f1-123">Đối với ứng dụng của bạn để truy nhập dữ liệu trong Microsoft graph, người dùng hoặc người quản trị phải cấp quyền chính xác thông qua quy trình chấp thuận.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="fe6f1-124">[Tham chiếu quyền đối với Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) liệt kê các quyền liên kết với mỗi bộ các API chính của Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="fe6f1-125">Nó cũng cung cấp hướng dẫn về cách sử dụng các quyền.</span><span class="sxs-lookup"><span data-stu-id="fe6f1-125">It also provides guidance about how to use the permissions.</span></span>
