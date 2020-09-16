---
title: thư mục 1336 RecoverableItems đã đầy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741289"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="9ab5f-102">Thư mục các mục có thể phục hồi được đầy đủ</span><span class="sxs-lookup"><span data-stu-id="9ab5f-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="9ab5f-103">Đối với hộp thư Exchange Online, giới hạn dung lượng lưu trữ mặc định cho thư mục các mục có thể phục hồi là 30 GB.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="9ab5f-104">Giới hạn lưu trữ cho thư mục các mục có thể phục hồi được tự động tăng lên 100 GB nếu hộp thư được đặt ở chế độ duy trì tranh chấp, hãy giữ khám phá điện tử hoặc được gán cho chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="9ab5f-105">Khi thư mục các mục có thể phục hồi đạt đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo những cách sau đây:</span><span class="sxs-lookup"><span data-stu-id="9ab5f-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="9ab5f-106">Người dùng không thể xóa bỏ các mục khỏi hộp thư.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="9ab5f-107">Trợ lý thư mục được quản lý không thể xóa các mục dựa trên thẻ lưu giữ hoặc thiết đặt thư mục được quản lý.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="9ab5f-108">Đối với các hộp thư có kích hoạt mục duy nhất được bật hoặc được đặt ở chế độ chờ, quy trình bảo vệ bản sao trên trang không thể duy trì các phiên bản của các mục do người dùng chỉnh sửa.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="9ab5f-109">Đối với hộp thư có bật ghi nhật ký kiểm tra hộp thư, không có mục nhập Nhật ký kiểm tra hộp thư nào có thể được lưu trong thư mục con trong thư mục các mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="9ab5f-110">Đối với hộp thư không ở trạng thái giữ, người quản trị có thể sử dụng `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lệnh trong Exchange Online PowerShell để xóa các mục trong thư mục các mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="9ab5f-111">Để biết thêm thông tin, hãy xem các chủ đề sau:</span><span class="sxs-lookup"><span data-stu-id="9ab5f-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="9ab5f-112">Tìm kiếm và xóa thư</span><span class="sxs-lookup"><span data-stu-id="9ab5f-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="9ab5f-113">Tìm kiếm-hộp thư</span><span class="sxs-lookup"><span data-stu-id="9ab5f-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="9ab5f-114">Đối với hộp thư đang ở trạng thái giữ, người quản trị phải loại bỏ giữ trước khi họ có thể xóa các mục khỏi thư mục các mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="9ab5f-115">Để biết thêm thông tin, hãy xem [mục xóa mục trong thư mục các mục có thể phục hồi của các hộp thư trên nền tảng điện toán đám mây](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9ab5f-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="9ab5f-116">Để ngăn không cho thư mục các mục có thể phục hồi trở nên đầy đủ, người quản trị có thể tăng giới hạn lưu trữ của thư mục các mục có thể phục hồi cho hộp thư khi giữ và thiết lập chính sách duy trì hộp thư di chuyển các mục từ thư mục các mục có thể phục hồi tới hộp thư lưu trữ của người dùng.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="9ab5f-117">Hãy xem [mục tăng hạn ngạch các mục có thể phục hồi cho hộp thư ở](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)chế độ chờ.</span><span class="sxs-lookup"><span data-stu-id="9ab5f-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
