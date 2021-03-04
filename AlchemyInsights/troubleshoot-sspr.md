---
title: Khắc phục sự cố SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430360"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="fb14d-102">Khắc phục sự cố SSPR</span><span class="sxs-lookup"><span data-stu-id="fb14d-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="fb14d-103">**Tôi đang gặp sự cố về cấu hình đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="fb14d-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="fb14d-104">Nếu bạn là người quản trị và tìm cách bật tính năng đặt lại mật khẩu tự phục vụ, hãy xem [hướng dẫn bật SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), để cấu hình đặt lại mật khẩu cho tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb14d-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="fb14d-105">Bạn cũng có thể muốn xem lại các [yêu cầu cấp phép](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fb14d-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="fb14d-106">Bạn phải có ít nhất một giấy phép được gán trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="fb14d-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="fb14d-107">**Đám mây chỉ người dùng** -bất kỳ Office 365 (O365) được trả về SKU hoặc Azure AD BASIC</span><span class="sxs-lookup"><span data-stu-id="fb14d-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="fb14d-108">Nền tảng điện **toán đám mây và/hoặc người dùng tại cơ sở** -Azure AD Premium P1 hoặc P2, doanh nghiệp Mobility + Security (EMS), hoặc doanh nghiệp hiệu quả bảo mật (SPE)</span><span class="sxs-lookup"><span data-stu-id="fb14d-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="fb14d-109">Để biết thêm thông tin về việc đặt lại mật khẩu tự phục vụ, hãy xem lại câu [hỏi thường gặp của chúng tôi](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fb14d-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="fb14d-110">**Tôi nhận được thông báo lỗi**</span><span class="sxs-lookup"><span data-stu-id="fb14d-110">**I'm getting an error message**</span></span>

<span data-ttu-id="fb14d-111">Xem lại bài viết này để tìm các lỗi thường gặp và giải pháp: [khắc phục sự cố đặt lại mật khẩu tự phục vụ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="fb14d-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="fb14d-112">**Tôi đang gặp sự cố với chính sách đặt lại mật khẩu của tôi**</span><span class="sxs-lookup"><span data-stu-id="fb14d-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="fb14d-113">Nếu chính sách đặt lại mật khẩu của bạn không phải là hành xử như mong muốn, hoặc nếu bạn có thắc mắc về chính sách đặt lại mật khẩu, hãy xem lại bài viết này: [chính sách mật khẩu và các hạn chế trong Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="fb14d-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="fb14d-114">Các chính sách đặt lại mật khẩu không áp dụng cho người quản trị.</span><span class="sxs-lookup"><span data-stu-id="fb14d-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="fb14d-115">Microsoft tham lực một chính sách đặt lại mật khẩu hai cổng mặc định mạnh cho bất kỳ vai trò người quản trị Azure nào.</span><span class="sxs-lookup"><span data-stu-id="fb14d-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="fb14d-116">Hãy đảm bảo rằng bạn đang thử nghiệm với người dùng không phải là người quản trị.</span><span class="sxs-lookup"><span data-stu-id="fb14d-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="fb14d-117">Để biết thêm thông tin về chính sách đặt lại người quản trị, hãy xem bài viết này: [sự khác biệt về chính sách đặt lại người quản trị](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span><span class="sxs-lookup"><span data-stu-id="fb14d-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="fb14d-118">**Tôi không muốn người dùng của mình đăng ký thông tin bảo mật bổ sung để đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="fb14d-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="fb14d-119">Bạn có thể có dữ liệu sẵn (email và thuộc tính điện thoại) cho người dùng của bạn bằng cách dùng API, PowerShell hoặc Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="fb14d-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="fb14d-120">Để tìm hiểu cách đọc:</span><span class="sxs-lookup"><span data-stu-id="fb14d-120">To learn how read:</span></span>

- [<span data-ttu-id="fb14d-121">Triển khai việc đặt lại mật khẩu mà không yêu cầu người dùng đăng ký</span><span class="sxs-lookup"><span data-stu-id="fb14d-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="fb14d-122">Việc đặt lại mật khẩu, dữ liệu nào được sử dụng</span><span class="sxs-lookup"><span data-stu-id="fb14d-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="fb14d-123">**Tôi muốn người dùng của mình đăng ký thông tin bảo mật bổ sung của họ để đặt lại mật khẩu**</span><span class="sxs-lookup"><span data-stu-id="fb14d-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="fb14d-124">Có người dùng của bạn đăng ký thông tin bảo mật của họ để đặt lại mật khẩu tự phục vụ bằng cách hướng họ đến [aka.MS/ssprsetup](https://mysignins.microsoft.com/security-info).</span><span class="sxs-lookup"><span data-stu-id="fb14d-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="fb14d-125">Sau khi dữ liệu được nhập cho người dùng (bởi người dùng hoặc người quản trị), hãy hướng dẫn người dùng của bạn đến [aka.MS/sspr](https://passwordreset.microsoftonline.com/) để người dùng của bạn có thể được quyền đặt lại mật khẩu của riêng họ.</span><span class="sxs-lookup"><span data-stu-id="fb14d-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="fb14d-126">Nếu người dùng vẫn gặp vấn đề mà họ có **thể liên** kết hoặc **mật khẩu Hash** người dùng đồng bộ.</span><span class="sxs-lookup"><span data-stu-id="fb14d-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="fb14d-127">Điều này có nghĩa là có vấn đề với dịch vụ Writeback mật khẩu.</span><span class="sxs-lookup"><span data-stu-id="fb14d-127">This means there is likely a problem with the Password Writeback service.</span></span>