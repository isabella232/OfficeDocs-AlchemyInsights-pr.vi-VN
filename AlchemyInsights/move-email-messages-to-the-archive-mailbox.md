---
title: Di chuyển thư email đến hộp thư lưu trữ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511062"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="c0736-102">Di chuyển email đến hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="c0736-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="c0736-103">Xác nhận rằng **hộp thư lưu trữ** đã được bật.</span><span class="sxs-lookup"><span data-stu-id="c0736-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="c0736-104">Nếu không, sử dụng các bước trong [bài viết này](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) để kích hoạt hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="c0736-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="c0736-105">Để lưu trữ thư tự động vào hộp thư lưu trữ, thẻ lưu giữ với hành động **di chuyển đến lưu trữ** phải được đặt **tự động áp dụng cho toàn bộ thẻ hộp thư (mặc định)**.</span><span class="sxs-lookup"><span data-stu-id="c0736-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="c0736-106">Sử dụng các bước ở đây để tạo thẻ: [lưu trữ thẻ mặc định](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="c0736-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="c0736-107">Tiếp theo, thêm thẻ **lưu trữ** vào chính sách lưu giữ của bạn.</span><span class="sxs-lookup"><span data-stu-id="c0736-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="c0736-108">Trong Trung tâm quản trị Exchange, chọn **chính sách lưu giữ** > thêm **di chuyển vào thẻ lưu trữ** chính sách > **lưu**.</span><span class="sxs-lookup"><span data-stu-id="c0736-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="c0736-109">Bây giờ [chỉ định chính sách lưu giữ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) cho hộp thư của người dùng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="c0736-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="c0736-110">Chính sách tương tự sẽ được áp dụng cho cả hộp thư **chính** và **lưu trữ** .</span><span class="sxs-lookup"><span data-stu-id="c0736-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="c0736-111">Nó có thể là cần thiết để buộc quản lý thư mục hỗ trợ (MFA) để chạy và áp dụng cài đặt mới cho hộp thư của người dùng.</span><span class="sxs-lookup"><span data-stu-id="c0736-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="c0736-112">Chạy lệnh sau khi [kết nối với eXo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) khởi động hỗ trợ thư mục được quản lý cho một hộp thư cụ thể:</span><span class="sxs-lookup"><span data-stu-id="c0736-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="c0736-113">Bắt đầu-ManagedFolderAssistant-Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="c0736-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="c0736-114">Để biết thêm thông tin về cách thiết lập chính sách lưu trữ, xem [thiết lập chính sách lưu trữ và xóa cho hộp thư](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="c0736-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  