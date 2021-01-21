---
title: Cấu hình và mở rộng thời gian có mã thông báo
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917201"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="53076-102">Cấu hình và mở rộng thời gian có mã thông báo</span><span class="sxs-lookup"><span data-stu-id="53076-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="53076-103">Bạn có thể xác định tuổi thọ của truy nhập, SAML hoặc ID mã thông báo do Microsoft Identity Platform phát hành.</span><span class="sxs-lookup"><span data-stu-id="53076-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="53076-104">Bạn có thể đặt các hạn token cho tất cả các ứng dụng trong tổ chức của mình, cho một ứng dụng nhiều đối tượng thuê (nhiều tổ chức) hoặc đối với một hiệu trưởng dịch vụ cụ thể trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="53076-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="53076-105">Để biết thêm thông tin, hãy đọc các [hạn của mã](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)thông báo cấu hình.</span><span class="sxs-lookup"><span data-stu-id="53076-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="53076-106">Ví dụ, đọc [ví dụ về cách cấu hình hạn của token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="53076-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="53076-107">Để tìm hiểu cách đặt cấu hình tuổi thọ và tính tương thích của mã thông báo trong Azure Active Directory B2C (Azure AD B2C), hãy xem mục [đặt cấu hình thẻ trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="53076-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="53076-108">Bài viết [cấu hình hành vi phiên trong Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) mô tả các phương pháp đăng nhập đơn (SSO) được sử dụng trong AZURE AD B2C và giúp bạn chọn phương pháp SSO thích hợp nhất khi cấu hình chính sách của bạn.</span><span class="sxs-lookup"><span data-stu-id="53076-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="53076-109">**Các thẻ mới có bao lâu? Chúng hợp lệ trong bao lâu?**</span><span class="sxs-lookup"><span data-stu-id="53076-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="53076-110">Token hạn là 1 giờ và tuổi thọ của phiên là 24 giờ.</span><span class="sxs-lookup"><span data-stu-id="53076-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="53076-111">Điều này có nghĩa là nếu không có yêu cầu nào được thực hiện trong 24 giờ, bạn sẽ cần phải đăng nhập lại trước khi yêu cầu mã thông báo mới.</span><span class="sxs-lookup"><span data-stu-id="53076-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="53076-112">Sau khi 30 tháng 5, 2020, không có đối tượng thuê mới sẽ có thể sử dụng chính sách Lifetime mã thông báo cấu hình để cấu hình phiên và làm mới các thẻ.</span><span class="sxs-lookup"><span data-stu-id="53076-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="53076-113">Việc việc phản đối sẽ xảy ra trong vài tháng sau đó, nghĩa là chúng tôi sẽ ngừng tôn phục phiên làm việc hiện tại và làm mới các phiếu ghi điểm.</span><span class="sxs-lookup"><span data-stu-id="53076-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="53076-114">Bạn vẫn có thể cấu hình Access hạn token sau khi deprecation.</span><span class="sxs-lookup"><span data-stu-id="53076-114">You can still configure access token lifetimes after the deprecation.</span></span>






