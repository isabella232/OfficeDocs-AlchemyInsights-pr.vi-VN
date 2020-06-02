---
title: 1336 RecoverableItems thư mục đầy đủ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510774"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="8a3af-102">Thư mục mục có thể phục hồi đầy đủ</span><span class="sxs-lookup"><span data-stu-id="8a3af-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="8a3af-103">Đối với hộp thư Exchange Online, giới hạn lưu trữ mặc định cho thư mục mục có thể phục hồi là 30 GB.</span><span class="sxs-lookup"><span data-stu-id="8a3af-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="8a3af-104">Giới hạn lưu trữ thư mục mục có thể phục hồi tự động tăng lên 100 GB nếu hộp thư được đặt trên tranh chấp giữ, eDiscovery giữ hoặc được gán cho chính sách lưu giữ.</span><span class="sxs-lookup"><span data-stu-id="8a3af-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="8a3af-105">Khi thư mục mục có thể phục hồi đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo các cách sau:</span><span class="sxs-lookup"><span data-stu-id="8a3af-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="8a3af-106">Người dùng không thể xoá các mục khỏi hộp thư.</span><span class="sxs-lookup"><span data-stu-id="8a3af-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="8a3af-107">Hỗ trợ thư mục quản lý không thể xoá các mục dựa trên thẻ lưu giữ hoặc cài đặt thư mục được quản lý.</span><span class="sxs-lookup"><span data-stu-id="8a3af-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="8a3af-108">Đối với hộp thư có phục hồi một mục kích hoạt hoặc được giữ lại, quá trình sao chép trên viết trang bảo vệ không thể duy trì phiên bản của mục được người dùng biên soạn.</span><span class="sxs-lookup"><span data-stu-id="8a3af-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="8a3af-109">Đối với hộp thư có hộp kiểm tra đăng nhập kích hoạt, không có mục nhập Nhật ký kiểm tra hộp thư có thể được lưu trong thư mục con kiểm toán trong cặp mục phục hồi.</span><span class="sxs-lookup"><span data-stu-id="8a3af-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="8a3af-110">Đối với hộp thư không tạm giữ, quản trị viên có thể sử dụng `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lệnh trong Exchange Online PowerShell để xoá các mục trong thư mục mục phục hồi.</span><span class="sxs-lookup"><span data-stu-id="8a3af-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="8a3af-111">Để biết thêm thông tin, hãy xem các chủ đề sau:</span><span class="sxs-lookup"><span data-stu-id="8a3af-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="8a3af-112">Tìm kiếm và xóa thư</span><span class="sxs-lookup"><span data-stu-id="8a3af-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="8a3af-113">Hộp thư tìm kiếm</span><span class="sxs-lookup"><span data-stu-id="8a3af-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="8a3af-114">Đối với hộp thư đang tạm giữ, quản trị viên phải loại bỏ việc giữ trước khi họ có thể xoá các mục khỏi thư mục mục phục hồi.</span><span class="sxs-lookup"><span data-stu-id="8a3af-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="8a3af-115">Để biết thêm thông tin, hãy xem [xóa các mục trong thư mục mục có thể phục hồi của hộp thư dựa trên ứng dụng web qua Internet trên giữ](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8a3af-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="8a3af-116">Để giúp ngăn không cho thư mục mục có thể phục hồi trở nên đầy đủ, quản trị viên sẽ tăng giới hạn lưu trữ của thư mục mục phục hồi cho hộp thư khi giữ và thiết lập chính sách lưu giữ hộp thư di chuyển các mục từ thư mục mục có thể phục hồi cho hộp thư lưu trữ của người dùng.</span><span class="sxs-lookup"><span data-stu-id="8a3af-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="8a3af-117">Xem [tăng dung lượng mục có thể phục hồi cho hộp thư đang giữ](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="8a3af-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
