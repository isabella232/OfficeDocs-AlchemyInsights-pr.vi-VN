---
title: Các sự cố khi phát triển ứng dụng
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974762"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="08291-102">Các sự cố khi phát triển ứng dụng</span><span class="sxs-lookup"><span data-stu-id="08291-102">Issues developing applications</span></span>

<span data-ttu-id="08291-103">Để khắc phục các sự cố phổ biến nhất khi tạo các ứng dụng Azure Active Directory (AD), hãy xem các bài viết sau đây:</span><span class="sxs-lookup"><span data-stu-id="08291-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="08291-104">Tôi gặp sự cố khi đăng nhập vào (các) ứng dụng chỉ sử dụng trình duyệt Chrome</span><span class="sxs-lookup"><span data-stu-id="08291-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="08291-105">Tôi không biết cách thay đổi mã thông báo mặc định cho ứng dụng của tôi</span><span class="sxs-lookup"><span data-stu-id="08291-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="08291-106">Tôi nhầm lẫn về cách thỏa thuận ứng dụng hoạt động</span><span class="sxs-lookup"><span data-stu-id="08291-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="08291-107">Tôi không biết cách cấp quyền đối với ứng dụng của mình</span><span class="sxs-lookup"><span data-stu-id="08291-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="08291-108">Tôi không hiểu sự khác biệt giữa quyền được ủy nhiệm và ứng dụng</span><span class="sxs-lookup"><span data-stu-id="08291-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="08291-109">\***Kết thúc hỗ trợ cho thư viện xác thực Azure Active Directory (ADAL) and AZURE AD GRAPH API (đồ họa Bad)** _</span><span class="sxs-lookup"><span data-stu-id="08291-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="08291-110">Bắt đầu từ ngày 30 tháng 6, 2020, chúng tôi sẽ không còn thêm bất kỳ tính năng nào mới vào thư viện xác thực Azure Active Directory (ADAL) và Azure AD graph API (đồ họa Bad).</span><span class="sxs-lookup"><span data-stu-id="08291-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="08291-111">Chúng tôi sẽ tiếp tục cung cấp hỗ trợ kỹ thuật và các bản Cập Nhật bảo mật nhưng sẽ không còn cung cấp các bản cập nhật tính năng.</span><span class="sxs-lookup"><span data-stu-id="08291-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="08291-112">Bắt đầu từ ngày 30 tháng 6, 2022, chúng tôi sẽ kết thúc hỗ trợ đối với đồ thị ADAL và Bad và sẽ không còn cung cấp hỗ trợ kỹ thuật hoặc các bản Cập Nhật bảo mật.</span><span class="sxs-lookup"><span data-stu-id="08291-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="08291-113">Do điều kiện này, sau đây là các tác động:</span><span class="sxs-lookup"><span data-stu-id="08291-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="08291-114">Ứng dụng bằng cách dùng ADAL trên các phiên bản hệ điều hành hiện có sẽ tiếp tục làm việc sau khi thời gian này nhưng sẽ không nhận được bất kỳ sự hỗ trợ kỹ thuật hoặc bản Cập Nhật bảo mật nào.</span><span class="sxs-lookup"><span data-stu-id="08291-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="08291-115">Các ứng dụng bằng cách sử dụng đồ thị Bad sau khi thời gian này không còn nhận được phản hồi từ điểm cuối của biểu đồ</span><span class="sxs-lookup"><span data-stu-id="08291-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="08291-116">*Di chuyển _ Adal*\*</span><span class="sxs-lookup"><span data-stu-id="08291-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="08291-117">Nếu bạn đang sử dụng ứng dụng Microsoft, chúng tôi khuyên bạn nên cập nhật lên thư viện xác thực Microsoft (MSAL), trong đó có các tính năng và bản Cập Nhật bảo mật mới nhất.</span><span class="sxs-lookup"><span data-stu-id="08291-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="08291-118">Đề xuất này nằm trong ngữ cảnh của Microsoft bắt đầu quá trình di chuyển ứng dụng của mình sang MSAL bằng hạn chót cuối cùng hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="08291-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="08291-119">Việc di chuyển theo Microsoft ứng dụng của nó vào MSAL đảm bảo rằng các ứng dụng sẽ lợi ích từ bảo mật và cải thiện tính năng của MSAL.</span><span class="sxs-lookup"><span data-stu-id="08291-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="08291-120">Đọc các câu hỏi thường gặp về ADAL</span><span class="sxs-lookup"><span data-stu-id="08291-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="08291-121">Tìm hiểu cách di chuyển các ứng dụng trên cơ sở mỗi nền tảng</span><span class="sxs-lookup"><span data-stu-id="08291-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="08291-122">Nếu bạn cần trợ giúp trong việc hiểu những ứng dụng của mình sử dụng ADAL, chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn, nếu có, hãy đến bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="08291-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="08291-123">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn một danh sách tất cả các ứng dụng không phải của Microsoft ADAL trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="08291-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="08291-124">**Di chuyển đồ thị trong Bad**</span><span class="sxs-lookup"><span data-stu-id="08291-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="08291-125">Đối với các ứng dụng đang sử dụng đồ thị Bad, hãy làm theo hướng dẫn của chúng tôi để di chuyển các ứng dụng đồ thị lên tiếng trên Microsoft graph:</span><span class="sxs-lookup"><span data-stu-id="08291-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="08291-126">[Danh sách kiểm tra di chuyển của chúng tôi cung cấp một điểm bắt đầu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="08291-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="08291-127">Cổng đăng ký Azure App của bạn hiển thị ứng dụng nào đang sử dụng đồ thị Bad.</span><span class="sxs-lookup"><span data-stu-id="08291-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="08291-128">Chúng tôi khuyên bạn nên xem xét tất cả mã nguồn của ứng dụng của bạn và nếu có, hãy tiếp cận với bất kỳ nhà cung cấp phần mềm độc lập nào (ISVs) hoặc nhà cung cấp ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="08291-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="08291-129">Hỗ trợ của Microsoft cũng có thể cung cấp cho bạn thông tin về việc sử dụng đồ thị trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="08291-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







