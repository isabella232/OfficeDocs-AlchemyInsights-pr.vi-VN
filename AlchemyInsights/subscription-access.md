---
title: Truy nhập thuê bao
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807727"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="38cf8-102">Không thể đăng nhập Azure do các sự cố của trình duyệt (trình duyệt bị treo, Giữ quay, không tải, v.v.)</span><span class="sxs-lookup"><span data-stu-id="38cf8-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="38cf8-103">Bạn có thể bị ảnh hưởng bởi sự mất điện.</span><span class="sxs-lookup"><span data-stu-id="38cf8-103">You might be impacted by an outage.</span></span> <span data-ttu-id="38cf8-104">Vui lòng kiểm tra xem liệu có đang mất liên tục không: [Azure trạng thái tình trạng](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="38cf8-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="38cf8-105">Vui lòng đăng xuất khỏi tất cả các phiên họp Azure hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="38cf8-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="38cf8-106">Bắt đầu chế độ một cách riêng tư hoặc ẩn danh trong trình duyệt web của bạn.</span><span class="sxs-lookup"><span data-stu-id="38cf8-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="38cf8-107">Bạn cũng có thể thử làm mới trình duyệt, sử dụng trình duyệt khác, xóa cookie bộ đệm ẩn nếu ở trên không hoạt động.</span><span class="sxs-lookup"><span data-stu-id="38cf8-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="38cf8-108">Tìm hiểu thêm: [khắc phục sự cố đăng nhập](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="38cf8-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="38cf8-109">**Không thể truy nhập đăng ký**</span><span class="sxs-lookup"><span data-stu-id="38cf8-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="38cf8-110">Trong [cổng thông tin Azure](https://portal.azure.com/), hãy đảm bảo rằng thư mục Azure đúng được chọn từ tài khoản ở phía trên cùng bên phải.</span><span class="sxs-lookup"><span data-stu-id="38cf8-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="38cf8-111">Trong [Trung tâm tài khoản Azure](https://account.windowsazure.com/Subscriptions), hãy đảm bảo rằng nếu tài khoản được sử dụng là người quản trị tài khoản.</span><span class="sxs-lookup"><span data-stu-id="38cf8-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="38cf8-112">Tìm hiểu thêm: [khắc phục sự cố không tìm thấy đăng ký](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="38cf8-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="38cf8-113">**Không thể truy nhập lịch sử thanh toán**</span><span class="sxs-lookup"><span data-stu-id="38cf8-113">**Unable to access billing history**</span></span>

<span data-ttu-id="38cf8-114">Người quản trị tài khoản cần phải đảm bảo rằng người dùng truy nhập thông tin thanh toán sẽ được thêm vào trong thư mục Azure Active Directory với tư cách là người dùng khách: [Thêm hoặc xóa người dùng mới](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38cf8-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="38cf8-115">Người dùng sau đó cần có vai trò quản trị toàn cầu: [gán vai trò cho người dùng](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38cf8-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="38cf8-116">Đăng bài này, người dùng có thể được truy nhập thanh toán bằng cách sử dụng chính sách RBAC: [cấp quyền truy nhập vào thanh toán](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="38cf8-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="38cf8-117">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="38cf8-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="38cf8-118">Tôi không thể đăng nhập để quản lý đăng ký Azure của tôi</span><span class="sxs-lookup"><span data-stu-id="38cf8-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)