---
title: Vai trò quản lý danh tính đặc quyền
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089146"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="60954-102">Vai trò quản lý danh tính đặc quyền (PIM)</span><span class="sxs-lookup"><span data-stu-id="60954-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="60954-103">**Quyền không được cấp sau khi kích hoạt một vai trò**</span><span class="sxs-lookup"><span data-stu-id="60954-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="60954-104">Khi bạn kích hoạt một vai trò trong Azure AD quản lý danh tính đặc quyền (PIM), kích hoạt có thể không được truyền ngay lập tức vào tất cả các cổng yêu cầu vai trò đặc quyền.</span><span class="sxs-lookup"><span data-stu-id="60954-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="60954-105">Đôi khi, ngay cả khi thay đổi được tuyên truyền, bộ đệm ẩn web trong một cổng thông tin có thể dẫn đến thay đổi này không có hiệu lực ngay lập tức.</span><span class="sxs-lookup"><span data-stu-id="60954-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="60954-106">Nếu kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="60954-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="60954-107">Đăng xuất khỏi cổng thông tin Azure và sau đó đăng nhập lại.</span><span class="sxs-lookup"><span data-stu-id="60954-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="60954-108">Khi bạn kích hoạt một vai trò Azure AD hoặc vai trò tài nguyên Azure, bạn sẽ thấy các giai đoạn của kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="60954-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="60954-109">Sau khi tất cả các giai đoạn hoàn tất, bạn sẽ thấy liên kết ' đăng xuất '.</span><span class="sxs-lookup"><span data-stu-id="60954-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="60954-110">Bạn có thể sử dụng liên kết này để đăng xuất. Việc này sẽ giải quyết hầu hết các trường hợp cho việc trì hoãn kích hoạt.</span><span class="sxs-lookup"><span data-stu-id="60954-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="60954-111">Trong PIM, hãy xác nhận rằng bạn được liệt kê là thành viên của vai trò đó.</span><span class="sxs-lookup"><span data-stu-id="60954-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="60954-112">Nếu bạn đang kích hoạt vai trò người quản trị Exchange, hãy đảm bảo rằng bạn đăng xuất và đăng nhập lại.</span><span class="sxs-lookup"><span data-stu-id="60954-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="60954-113">Nếu sự cố vẫn tiếp diễn, hãy mở một vé hỗ trợ và nâng cao này làm vấn đề.</span><span class="sxs-lookup"><span data-stu-id="60954-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="60954-114">Nếu bạn đang sử dụng vai trò người quản trị Exchange của mình để truy nhập vào Trung tâm bảo mật và tuân thủ, hãy xem bước tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="60954-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="60954-115">Nếu bạn đang kích hoạt một vai trò để truy nhập vào Trung tâm bảo mật và tuân thủ hoặc nếu bạn đang kích hoạt vai trò người quản trị SharePoint, bạn sẽ gặp một số trì hoãn kích hoạt từ vài phút lên đến vài giờ.</span><span class="sxs-lookup"><span data-stu-id="60954-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="60954-116">Đây là một vấn đề đã biết và chúng tôi đang tích cực làm việc với các nhóm này để giải quyết sự cố này càng sớm càng tốt.</span><span class="sxs-lookup"><span data-stu-id="60954-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="60954-117">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="60954-117">For more information, see:</span></span>

- [<span data-ttu-id="60954-118">Kích hoạt Azure AD Roles của tôi trong PIM</span><span class="sxs-lookup"><span data-stu-id="60954-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="60954-119">Kích hoạt các vai trò tài nguyên Azure của tôi trong PIM</span><span class="sxs-lookup"><span data-stu-id="60954-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="60954-120">**Quyền không bị loại bỏ sau khi hủy kích hoạt một vai trò hoặc kích hoạt vai trò hết hạn**</span><span class="sxs-lookup"><span data-stu-id="60954-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="60954-121">Khi bạn hủy kích hoạt một vai trò trong quản lý căn cước có đặc quyền Azure AD hoặc khi nào hết hạn, có thể có một sự chậm trễ mà bạn tiếp tục có quyền truy nhập.</span><span class="sxs-lookup"><span data-stu-id="60954-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="60954-122">Nếu hủy kích hoạt của bạn bị trì hoãn, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="60954-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="60954-123">Nếu bạn đang hủy kích hoạt vai trò người quản trị Exchange hoặc thời hạn kích hoạt vai trò hết hạn, và bạn nhận thấy sự chậm trễ đáng kể trước khi các quyền được loại bỏ, hãy mở một vé hỗ trợ và thông báo cho kỹ sư hỗ trợ của bạn để giúp bạn gửi một vé với nhóm quản lý truy nhập đặc quyền (PAM) trong Office về vấn đề này.</span><span class="sxs-lookup"><span data-stu-id="60954-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="60954-124">Nếu thời gian kích hoạt đã hết hạn, nhưng bạn vẫn đang mở phiên trình duyệt, hãy đóng trình duyệt của bạn.</span><span class="sxs-lookup"><span data-stu-id="60954-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="60954-125">Bạn có thể tiếp tục sử dụng vai trò cho đến khi bạn đóng phiên đó.</span><span class="sxs-lookup"><span data-stu-id="60954-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="60954-126">Đây là một vấn đề đã biết và chúng tôi đang tìm kiếm một bản sửa lỗi nhằm kích hoạt lại mỗi phiên đã hết hạn.</span><span class="sxs-lookup"><span data-stu-id="60954-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="60954-127">Nếu sự chậm trễ của bạn khác với hai kịch bản này, vui lòng mở một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="60954-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
