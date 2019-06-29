---
title: 1336 RecoverableItems thư mục là đầy đủ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 05e7b47a2200c3b0500e7d786166966ea301179a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35370409"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="c8609-102">Thư mục mục có thể phục hồi được đầy đủ</span><span class="sxs-lookup"><span data-stu-id="c8609-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="c8609-103">Đối với hộp thư Exchange Online trong Office 365, giới hạn dung lượng mặc định cho thư mục mục có thể phục hồi là 30 GB.</span><span class="sxs-lookup"><span data-stu-id="c8609-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="c8609-104">Giới hạn lưu trữ cho thư mục mục có thể phục hồi tự động tăng lên tới 100 GB nếu hộp thư được đặt trên tranh chấp giữ, Giữ lại eDiscovery, hoặc được gán cho một chính sách lưu giữ Office 365.</span><span class="sxs-lookup"><span data-stu-id="c8609-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="c8609-105">Khi thư mục mục có thể phục hồi đạt đến giới hạn lưu trữ, chức năng hộp thư bị ảnh hưởng theo các cách sau:</span><span class="sxs-lookup"><span data-stu-id="c8609-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="c8609-106">Người dùng không thể xoá các mục khỏi hộp thư.</span><span class="sxs-lookup"><span data-stu-id="c8609-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="c8609-107">Chương trình hỗ trợ thư mục quản lý không thể xoá các mục dựa trên thẻ lưu giữ hoặc cài đặt thư mục được quản lý.</span><span class="sxs-lookup"><span data-stu-id="c8609-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="c8609-108">Cho hộp thư đã khôi phục từng mục duy nhất kích hoạt hoặc được đặt trên giữ, quá trình bảo vệ bản sao trên viết trang không thể duy trì các phiên bản của bài chỉnh sửa của người dùng.</span><span class="sxs-lookup"><span data-stu-id="c8609-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="c8609-109">Cho các hộp thư có hộp thư được kích hoạt ghi nhật ký kiểm tra, không có mục nào đăng nhập hộp thư kiểm tra có thể được lưu trong thư mục kiểm tra trong thư mục mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="c8609-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="c8609-110">Hộp thư không phải là tổ chức, quản trị viên có thể sử dụng các `Search-Mailbox -SearchDumpsterOnly -DeleteContent` lệnh trong Exchange Online PowerShell để xóa các khoản mục trong thư mục mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="c8609-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="c8609-111">Để biết thêm thông tin, hãy xem các chủ đề sau:</span><span class="sxs-lookup"><span data-stu-id="c8609-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="c8609-112">Tìm kiếm và xoá thư</span><span class="sxs-lookup"><span data-stu-id="c8609-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="c8609-113">Hộp thư tìm kiếm</span><span class="sxs-lookup"><span data-stu-id="c8609-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="c8609-114">Cho các hộp thư về tổ chức, quản trị viên có để loại bỏ các giữ trước khi họ có thể các khoản mục đã xóa khỏi thư mục mục có thể phục hồi.</span><span class="sxs-lookup"><span data-stu-id="c8609-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="c8609-115">Để biết thêm chi tiết, hãy xem [xóa các khoản mục trong các mục có thể phục hồi các thư mục trong hộp thư dựa trên giữ](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c8609-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="c8609-116">Để giúp ngăn ngừa thư mục mục có thể phục hồi từ trở nên đầy đủ, quản trị viên có thể tăng giới hạn lưu trữ các mục có thể phục hồi các thư mục hộp thư vào tổ chức và thiết lập một chính sách lưu giữ hộp thư di chuyển khoản mục khỏi thư mục mục có thể phục hồi để lưu trữ của người dùng hộp thư.</span><span class="sxs-lookup"><span data-stu-id="c8609-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="c8609-117">Thấy [tăng các khoản mục có thể phục hồi định mức cho hộp thư trên tổ chức](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="c8609-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
