---
title: Outlook Desktop nhớ lại hoặc thay thế một thư email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 3d3a6c253317137b7069a978b907c97d61bf7313
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/15/2019
ms.locfileid: "36496133"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="23db7-102">Gọi lại hoặc thay thế thư email Outlook</span><span class="sxs-lookup"><span data-stu-id="23db7-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="23db7-103">Là quản trị viên, bạn có thể **nhớ lại thư thay mặt người dùng sử dụng PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="23db7-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="23db7-104">Bạn không thể gọi lại thư từ Trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="23db7-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="23db7-105">Bạn chỉ có thể **gọi lại thư được gửi cho những người trong tổ chức của bạn**.</span><span class="sxs-lookup"><span data-stu-id="23db7-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="23db7-106">Ví dụ: nếu thư được gửi đến địa chỉ Gmail, bạn không thể gọi lại thông báo đó.</span><span class="sxs-lookup"><span data-stu-id="23db7-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="23db7-107">Bạn chỉ có thể **gọi lại thư được gửi từ Outlook 2016 trên PC**.</span><span class="sxs-lookup"><span data-stu-id="23db7-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="23db7-108">Nếu người dùng gửi thư bằng cách sử dụng Outlook dành cho Mac hoặc Outlook trên web, bạn không thể gọi lại.</span><span class="sxs-lookup"><span data-stu-id="23db7-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="23db7-109">Để gọi lại hoặc thay thế thư email:</span><span class="sxs-lookup"><span data-stu-id="23db7-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="23db7-110">Trong ngăn thư mục bên trái cửa sổ Outlook, chọn thư mục mục đã gửi.</span><span class="sxs-lookup"><span data-stu-id="23db7-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="23db7-111">Bấm đúp vào thư bạn muốn gọi lại để mở.</span><span class="sxs-lookup"><span data-stu-id="23db7-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="23db7-112">Chọn tab **thông báo** , sau đó chọn **hành động** > thu**hồi thông báo này**.</span><span class="sxs-lookup"><span data-stu-id="23db7-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="23db7-113">Chọn **xóa các bản sao chưa đọc của thư này** hoặc **xóa các bản sao chưa đọc và thay thế bằng một tin nhắn mới**, sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="23db7-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="23db7-114">Nếu bạn đang gửi một tin nhắn thay thế, soạn tin nhắn, và sau đó chọn **gửi**.</span><span class="sxs-lookup"><span data-stu-id="23db7-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="23db7-115">Sự thành công hay thất bại của một tin nhắn thu hồi phụ thuộc vào cài đặt của người nhận trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="23db7-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="23db7-116">Để biết các bước kiểm tra thu hồi, hãy xem [bài viết này](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="23db7-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="23db7-117">Tìm kiếm và xóa thư email trong tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="23db7-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="23db7-118">Nếu bạn không phải là quản trị viên toàn cầu, tài khoản của bạn cần được thêm vào vai trò của trình quản lý eDiscovery hoặc vai trò quản lý tìm kiếm phù hợp để tìm kiếm thư.</span><span class="sxs-lookup"><span data-stu-id="23db7-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="23db7-119">Để xóa thư, bạn sẽ cần tham gia nhóm vai trò quản lý tổ chức hoặc vai trò quản lý tìm kiếm và dọn sạch.</span><span class="sxs-lookup"><span data-stu-id="23db7-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="23db7-120">Quyền cho các vai trò được chỉ định trong [Trung tâm bảo mật và tuân thủ](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="23db7-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="23db7-121">[Tạo tìm kiếm nội dung](https://docs.microsoft.com/office365/securitycompliance/content-search) để tìm thư cần xóa.</span><span class="sxs-lookup"><span data-stu-id="23db7-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="23db7-122">[Kết nối với PowerShell Trung tâm bảo mật và tuân thủ](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="23db7-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="23db7-123">Nếu bạn đang sử dụng xác thực nhiều yếu tố, hãy xem [kết nối với Office 365 Trung tâm bảo mật và tuân thủ PowerShell bằng cách sử dụng xác thực nhiều yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="23db7-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>