---
title: Ứng dụng xác thực
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405686"
---
# <a name="authentication-app"></a><span data-ttu-id="5d8d0-102">Ứng dụng xác thực</span><span class="sxs-lookup"><span data-stu-id="5d8d0-102">Authentication app</span></span>

<span data-ttu-id="5d8d0-103">Nếu bạn là người quản trị toàn cầu, bạn có thể nhanh chóng tìm hiểu điều gì đã xảy ra hoặc chẩn đoán các vấn đề liên quan đến người dùng đăng nhập bằng cách sử dụng [chẩn đoán đăng nhập](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="5d8d0-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="5d8d0-104">Bắt đầu chẩn đoán bằng cách bấm nút "[khởi động chẩn đoán](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)".</span><span class="sxs-lookup"><span data-stu-id="5d8d0-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="5d8d0-105">Tìm sự kiện để phân tích bằng cách nhập vào các chi tiết bạn có về người dùng, ứng dụng, thời gian đăng nhập, yêu cầu ID hoặc tương quan ID.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="5d8d0-106">Xem lại kết quả chẩn đoán Hiển thị chi tiết về những điều đã xảy ra và những hành động bạn có thể thực hiện để thay đổi, nếu bất kỳ thay đổi nào cần thiết.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="5d8d0-107">**Kiểm tra tình huống được áp dụng:**</span><span class="sxs-lookup"><span data-stu-id="5d8d0-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="5d8d0-108">Nếu người dùng không nhận được thông báo đẩy trong ứng dụng Microsoft Authenticator, hãy xác minh rằng họ không được hiển thị bên dưới người dùng bị chặn MFA như được mô tả trong [khối và bỏ chặn người dùng](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="5d8d0-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="5d8d0-109">Nếu người dùng không bị chặn đối với MFA nhưng không nhận được thông báo đẩy, họ có thể mở ứng dụng Microsoft Authenticator, vốn sẽ kéo các yêu cầu phê duyệt đang chờ xử lý.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="5d8d0-110">Là phương pháp đăng nhập thay thế, người dùng cũng có thể bấm vào đăng nhập theo cách khác và chọn sử dụng mã xác minh từ ứng dụng dành cho thiết bị di động của tôi.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="5d8d0-111">Ứng dụng Microsoft Authenticator là phương thức sẵn dùng duy nhất cho nhiều người dùng.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="5d8d0-112">[Tìm hiểu thêm về mặc định bảo mật](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), hãy chọn câu hỏi [thường gặp về ứng dụng](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) xác thực cho các câu hỏi thường gặp và cách giải quyết chúng.</span><span class="sxs-lookup"><span data-stu-id="5d8d0-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="5d8d0-113">**Video được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="5d8d0-113">**Recommended Videos**</span></span>

<span data-ttu-id="5d8d0-114">[Cách thiết lập ứng dụng Authenticator trên điện thoại mới (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5d8d0-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
