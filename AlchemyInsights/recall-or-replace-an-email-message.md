---
title: Thu hồi hoặc thay thế thông điệp email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353528"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="71f51-102">Thu hồi hoặc thay thế thông điệp email trong Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="71f51-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="71f51-103">Bạn chỉ có thể thu **hồi thư được gửi đến những người trong tổ chức của bạn**.</span><span class="sxs-lookup"><span data-stu-id="71f51-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="71f51-104">Ví dụ, nếu thư đã được gửi đến một địa chỉ Gmail, bạn không thể thu hồi thư.</span><span class="sxs-lookup"><span data-stu-id="71f51-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="71f51-105">Bạn chỉ có thể **gọi lại các thư được gửi từ Outlook cho PC**.</span><span class="sxs-lookup"><span data-stu-id="71f51-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="71f51-106">Nếu người dùng gửi thư bằng cách dùng Outlook cho Mac hoặc Outlook trên web, bạn không thể thu hồi thư.</span><span class="sxs-lookup"><span data-stu-id="71f51-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="71f51-107">Là người quản trị đối tượng thuê, bạn có thể thu **hồi thư thay mặt cho người dùng bằng cách sử dụng PowerShell** (để biết thêm thông tin, hãy xem: [Tìm kiếm và xóa thông điệp email](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="71f51-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="71f51-108">Bạn không thể thu hồi thư từ Trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="71f51-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="71f51-109">Cuộn xuống đến "tìm kiếm và xóa thông điệp email trong tổ chức của bạn" để biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="71f51-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="71f51-110">**Thu hồi hoặc thay thế thông điệp email mà bạn đã gửi**</span><span class="sxs-lookup"><span data-stu-id="71f51-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="71f51-111">Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục các mục đã gửi.</span><span class="sxs-lookup"><span data-stu-id="71f51-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="71f51-112">Mở thư mà bạn muốn thu hồi.</span><span class="sxs-lookup"><span data-stu-id="71f51-112">Open the message that you want to recall.</span></span> <span data-ttu-id="71f51-113">Bạn phải bấm đúp để mở thư.</span><span class="sxs-lookup"><span data-stu-id="71f51-113">You must double-click to open the message.</span></span> <span data-ttu-id="71f51-114">Chọn thư để nó xuất hiện trong ngăn đọc sẽ không cho phép bạn thu hồi thư.</span><span class="sxs-lookup"><span data-stu-id="71f51-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="71f51-115">Từ tab thư, chọn **hành động** thu  >  **hồi thư này**.</span><span class="sxs-lookup"><span data-stu-id="71f51-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="71f51-116">Chọn **xóa bỏ các bản sao chưa đọc của thư này** hoặc **xóa bỏ các bản sao chưa đọc và thay thế bằng thư mới**, rồi chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="71f51-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="71f51-117">Nếu bạn đang gửi một thông báo thay thế, hãy soạn thư, rồi chọn **gửi**.</span><span class="sxs-lookup"><span data-stu-id="71f51-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="71f51-118">Sự thành công hay thất bại của thư được thu hồi tùy thuộc vào cài đặt của người nhận trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="71f51-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="71f51-119">Để biết thêm thông tin, bao gồm cách kiểm tra việc thu hồi, hãy xem thu [hồi hoặc thay thế thông điệp email mà bạn đã gửi](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="71f51-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="71f51-120">**_Để tìm kiếm và xóa thông điệp email trong tổ chức của bạn_**, bạn nên dễ dàng nhất nếu bạn là người quản trị toàn cầu. Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào nhóm vai trò trình quản lý khám phá điện tử hoặc đối với vai trò quản lý tìm kiếm tuân thủ.</span><span class="sxs-lookup"><span data-stu-id="71f51-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="71f51-121">Để xóa thư, bạn sẽ cần phải tham gia vào nhóm vai trò quản lý tổ chức hoặc vai trò tìm kiếm và dọn sạch quản lý.</span><span class="sxs-lookup"><span data-stu-id="71f51-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="71f51-122">Quyền đối với các vai trò này được gán trong [Trung tâm tuân thủ & bảo mật](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="71f51-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="71f51-123">[Tạo một tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/content-search) để tìm thư cần xóa.</span><span class="sxs-lookup"><span data-stu-id="71f51-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="71f51-124">[Kết nối với Trung tâm bảo mật & PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="71f51-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="71f51-125">Nếu bạn đang sử dụng MFA (xác thực đa yếu tố), hãy xem [kết nối với Trung tâm bảo mật của Microsoft 365 & PowerShell bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="71f51-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
