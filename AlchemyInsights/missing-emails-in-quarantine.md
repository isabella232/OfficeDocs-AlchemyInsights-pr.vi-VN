---
title: Thiếu email trong cách ly
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831756"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="1bdca-102">Thiếu email trong cách ly "</span><span class="sxs-lookup"><span data-stu-id="1bdca-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="1bdca-103">Người quản trị có thể [xem, phát hành hoặc xóa các thư này.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="1bdca-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="1bdca-104">Để mở Trung tâm tuân thủ & bảo mật, hãy đi tới [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="1bdca-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="1bdca-105">Để mở trực tiếp trang cách ly, hãy đi đến [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="1bdca-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="1bdca-106">Bạn có thể tìm kiếm theo các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="1bdca-106">You can search by the following values:</span></span>  

- <span data-ttu-id="1bdca-107">**ID thông báo: mã** định danh duy nhất trên toàn cầu của thư.</span><span class="sxs-lookup"><span data-stu-id="1bdca-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="1bdca-108">Nếu bạn chọn một thư trong danh sách, giá trị  **ID thông báo**  sẽ xuất hiện trong ngăn  **thông tin chi tiết**  xuất hiện.</span><span class="sxs-lookup"><span data-stu-id="1bdca-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="1bdca-109">Người quản trị có thể sử dụng theo [dõi thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) để tìm thư và các giá trị ID thông báo tương ứng của chúng.</span><span class="sxs-lookup"><span data-stu-id="1bdca-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="1bdca-110">**Địa chỉ email người gửi**: địa chỉ email của một người gửi.</span><span class="sxs-lookup"><span data-stu-id="1bdca-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="1bdca-111">**Địa chỉ email người nhận**: địa chỉ email của một người nhận.</span><span class="sxs-lookup"><span data-stu-id="1bdca-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="1bdca-112">**Subject**: dùng toàn bộ chủ đề của thư.</span><span class="sxs-lookup"><span data-stu-id="1bdca-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="1bdca-113">Tìm kiếm không phân biệt chữ hoa/thường.</span><span class="sxs-lookup"><span data-stu-id="1bdca-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="1bdca-114">Sau khi bạn đã nhập tiêu chí tìm kiếm, bấm làm mới nút làm mới ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  để lọc kết quả.  </span><span class="sxs-lookup"><span data-stu-id="1bdca-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="1bdca-115">Các lệnh ghép ngắn mà bạn sử dụng để xem và quản lý các thư và tệp trong cách ly:</span><span class="sxs-lookup"><span data-stu-id="1bdca-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="1bdca-116">Xóa-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1bdca-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="1bdca-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1bdca-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="1bdca-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1bdca-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="1bdca-119">Bản [xem trước-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): lưu ý rằng lệnh ghép ngắn này chỉ dành cho các thư, không phải tệp phần mềm độc hại từ ATP cho SharePoint Online, OneDrive for Business hoặc nhóm.</span><span class="sxs-lookup"><span data-stu-id="1bdca-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="1bdca-120">Bản phát hành-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="1bdca-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)