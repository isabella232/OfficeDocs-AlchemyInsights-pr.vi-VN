---
title: Outlook Desktop thu hồi hoặc thay thế thông điệp email
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664012"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="a9ce6-102">Thu hồi hoặc thay thế thông điệp email Outlook</span><span class="sxs-lookup"><span data-stu-id="a9ce6-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="a9ce6-103">Với tư cách là người quản trị, bạn có thể thu **hồi thư thay mặt cho người dùng bằng PowerShell**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="a9ce6-104">Bạn không thể thu hồi thư từ Trung tâm quản trị.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="a9ce6-105">Bạn chỉ có thể thu **hồi thư được gửi đến những người trong tổ chức của bạn**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="a9ce6-106">Ví dụ: nếu thư đã được gửi đến một địa chỉ Gmail, chẳng hạn như bạn không thể thu hồi nó.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="a9ce6-107">Bạn chỉ có thể **gọi lại các thư được gửi từ Outlook 2016 trên PC**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="a9ce6-108">Nếu người dùng gửi thư bằng cách dùng Outlook cho Mac hoặc Outlook trên web, bạn không thể thu hồi thư.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="a9ce6-109">Để thu hồi hoặc thay thế thông điệp email:</span><span class="sxs-lookup"><span data-stu-id="a9ce6-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="a9ce6-110">Trong ngăn thư mục ở bên trái của cửa sổ Outlook, chọn thư mục các mục đã gửi.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="a9ce6-111">Bấm đúp vào thư mà bạn muốn thu hồi để mở.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="a9ce6-112">Chọn tab **thư** , rồi chọn **hành động**thu  >  **hồi thư này**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="a9ce6-113">Chọn **xóa bỏ các bản sao chưa đọc của thư này** hoặc **xóa bỏ các bản sao chưa đọc và thay thế bằng thư mới**, rồi chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="a9ce6-114">Nếu bạn đang gửi một thông báo thay thế, soạn thư, rồi chọn **gửi**.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="a9ce6-115">Sự thành công hoặc thất bại của thư được thu hồi tùy thuộc vào cài đặt của người nhận trong Outlook.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="a9ce6-116">Để biết các bước kiểm tra lại, hãy xem [bài viết này](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="a9ce6-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="a9ce6-117">Tìm kiếm và xóa thông điệp email trong tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="a9ce6-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="a9ce6-118">Nếu bạn không phải là người quản trị toàn cầu, tài khoản của bạn phải được thêm vào vai trò quản lý khám phá điện tử hoặc vai trò tìm kiếm tuân thủ để tìm kiếm thư.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="a9ce6-119">Để xóa thư, bạn sẽ cần phải tham gia vào nhóm vai trò quản lý tổ chức hoặc vai trò tìm kiếm và dọn sạch quản lý.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="a9ce6-120">Quyền cho các vai trò này được gán trong [Trung tâm bảo mật và tuân thủ](https://go.microsoft.com/fwlink/?linkid=2083731).</span><span class="sxs-lookup"><span data-stu-id="a9ce6-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="a9ce6-121">[Tạo một tìm kiếm nội dung](https://docs.microsoft.com/microsoft-365/compliance/content-search) để tìm thư cần xóa.</span><span class="sxs-lookup"><span data-stu-id="a9ce6-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="a9ce6-122">[Kết nối với Trung tâm bảo mật và tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="a9ce6-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="a9ce6-123">Nếu bạn đang sử dụng xác thực đa yếu tố, hãy xem [kết nối với Trung tâm bảo mật và tuân thủ Microsoft 365 bằng cách dùng xác thực đa yếu tố](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="a9ce6-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>