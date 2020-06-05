---
title: Thiếu email trong cách ly
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569565"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="665c5-102">Thiếu email trong kiểm dịch "</span><span class="sxs-lookup"><span data-stu-id="665c5-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="665c5-103">Quản trị viên có thể [xem, phát hành hoặc xoá các thư này.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="665c5-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="665c5-104">Để mở Trung tâm tuân thủ & bảo mật, hãy chuyển đến [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="665c5-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="665c5-105">Để mở trực tiếp trang cách ly, hãy chuyển đến [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="665c5-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="665c5-106">Bạn có thể tìm kiếm theo các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="665c5-106">You can search by the following values:</span></span>  

- <span data-ttu-id="665c5-107">**Message ID**: mã định danh duy nhất toàn cầu của thư.</span><span class="sxs-lookup"><span data-stu-id="665c5-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="665c5-108">Nếu bạn chọn một thư trong danh sách, giá trị **ID thư** sẽ xuất hiện trong ngăn hộp thả xuống **chi tiết** xuất hiện.</span><span class="sxs-lookup"><span data-stu-id="665c5-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="665c5-109">Quản trị viên có thể sử dụng [theo dõi thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) để tìm thư và các giá trị Message ID tương ứng.</span><span class="sxs-lookup"><span data-stu-id="665c5-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="665c5-110">**Địa chỉ email người gửi**: một địa chỉ email của người gửi duy nhất.</span><span class="sxs-lookup"><span data-stu-id="665c5-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="665c5-111">**Địa chỉ email người nhận**: địa chỉ email của một người nhận.</span><span class="sxs-lookup"><span data-stu-id="665c5-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="665c5-112">**Chủ**đề: sử dụng toàn bộ chủ đề của tin nhắn.</span><span class="sxs-lookup"><span data-stu-id="665c5-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="665c5-113">Tìm kiếm không phải là chữ.</span><span class="sxs-lookup"><span data-stu-id="665c5-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="665c5-114">Sau khi bạn đã nhập tiêu chí tìm kiếm, hãy nhấp vào Refresh ![ nút ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** để lọc kết quả.  </span><span class="sxs-lookup"><span data-stu-id="665c5-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="665c5-115">Các lệnh ghép ngắn bạn sử dụng để xem và quản lý thư và tệp cách ly là:</span><span class="sxs-lookup"><span data-stu-id="665c5-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="665c5-116">Xóa-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="665c5-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="665c5-117">Xuất-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="665c5-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="665c5-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="665c5-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="665c5-119">[Xem trước-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): lưu ý rằng lệnh này chỉ dành cho các thư, không phải tệp phần mềm độc hại từ ATP cho SharePoint Online, OneDrive for Business hoặc teams.</span><span class="sxs-lookup"><span data-stu-id="665c5-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="665c5-120">Phát hành-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="665c5-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)