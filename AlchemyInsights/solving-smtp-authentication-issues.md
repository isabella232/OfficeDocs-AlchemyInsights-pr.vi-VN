---
title: Bật xác thực và khắc phục sự cố SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077673"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="a7e73-102">Bật xác thực và khắc phục sự cố SMTP</span><span class="sxs-lookup"><span data-stu-id="a7e73-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="a7e73-103">Nếu bạn muốn bật xác thực SMTP cho một hộp thư hoặc bạn đang nhận được một "Máy khách chưa được xác thực", Lỗi "Xác thực không thành công" hoặc lỗi "SmtpClientAuthentication" với mã 5.7.57 hoặc 5.7.3 hoặc 5.7.139 khi bạn cố gắng chuyển tiếp email bằng cách xác thực một thiết bị hoặc ứng dụng với Microsoft 365, hãy thực hiện ba hành động này để giải quyết vấn đề này:</span><span class="sxs-lookup"><span data-stu-id="a7e73-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="a7e73-104">Tắt mặc [định bảo mật Azure bằng](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) cách chuyển Bật mặc định bảo **mật** thành **Không.**</span><span class="sxs-lookup"><span data-stu-id="a7e73-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="a7e73-105">a.</span><span class="sxs-lookup"><span data-stu-id="a7e73-105">a.</span></span> <span data-ttu-id="a7e73-106">Đăng nhập vào cổng thông tin Azure với tư cách người quản trị Bảo mật, người quản trị Truy nhập có Điều kiện hoặc người quản trị toàn cầu.</span><span class="sxs-lookup"><span data-stu-id="a7e73-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="a7e73-107">b.</span><span class="sxs-lookup"><span data-stu-id="a7e73-107">b.</span></span> <span data-ttu-id="a7e73-108">Duyệt đến Thuộc Azure Active Directory > **tính.**</span><span class="sxs-lookup"><span data-stu-id="a7e73-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="a7e73-109">c.</span><span class="sxs-lookup"><span data-stu-id="a7e73-109">c.</span></span> <span data-ttu-id="a7e73-110">Chọn **Quản lý mặc định bảo mật**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="a7e73-111">d.</span><span class="sxs-lookup"><span data-stu-id="a7e73-111">d.</span></span> <span data-ttu-id="a7e73-112">Đặt **Bật mặc định bảo mật** là **Không**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="a7e73-113">e.</span><span class="sxs-lookup"><span data-stu-id="a7e73-113">e.</span></span> <span data-ttu-id="a7e73-114">Chọn **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-114">Select **Save**.</span></span>

2. <span data-ttu-id="a7e73-115">[Bật gửi SMTP máy khách trên](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) hộp thư được cấp phép.</span><span class="sxs-lookup"><span data-stu-id="a7e73-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="a7e73-116">a.</span><span class="sxs-lookup"><span data-stu-id="a7e73-116">a.</span></span> <span data-ttu-id="a7e73-117">Từ hộp Trung tâm quản trị Microsoft 365, đi tới **Người dùng Hiện hoạt**, rồi chọn người dùng.</span><span class="sxs-lookup"><span data-stu-id="a7e73-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="a7e73-118">b.</span><span class="sxs-lookup"><span data-stu-id="a7e73-118">b.</span></span> <span data-ttu-id="a7e73-119">Đi tới tab Thư và trong Ứng dụng **email**, chọn Quản **lý ứng dụng email**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="a7e73-120">d.</span><span class="sxs-lookup"><span data-stu-id="a7e73-120">d.</span></span> <span data-ttu-id="a7e73-121">Đảm bảo đã chọn (đã bật xác thực **SMTP).**</span><span class="sxs-lookup"><span data-stu-id="a7e73-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="a7e73-122">e.</span><span class="sxs-lookup"><span data-stu-id="a7e73-122">e.</span></span> <span data-ttu-id="a7e73-123">Chọn **Lưu thay đổi**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="a7e73-124">[Tắt Xác thực Đa Yếu tố (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) trên hộp thư được cấp phép.</span><span class="sxs-lookup"><span data-stu-id="a7e73-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="a7e73-125">a.</span><span class="sxs-lookup"><span data-stu-id="a7e73-125">a.</span></span> <span data-ttu-id="a7e73-126">Đi tới menu Trung tâm quản trị Microsoft 365, rồi trong menu dẫn hướng bên trái, chọn Người dùng **người dùng**  >  **hiện hoạt**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="a7e73-127">b.</span><span class="sxs-lookup"><span data-stu-id="a7e73-127">b.</span></span> <span data-ttu-id="a7e73-128">Chọn **Xác thực đa yếu tố**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="a7e73-129">c.</span><span class="sxs-lookup"><span data-stu-id="a7e73-129">c.</span></span> <span data-ttu-id="a7e73-130">Chọn người dùng, rồi tắt **xác thực Đa Yếu tố**.</span><span class="sxs-lookup"><span data-stu-id="a7e73-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
