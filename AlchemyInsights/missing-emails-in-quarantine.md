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
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539846"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="e5fab-102">Thiếu email trong cách ly"</span><span class="sxs-lookup"><span data-stu-id="e5fab-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="e5fab-103">Người quản trị có [thể xem, phát hành hoặc xóa bỏ những thông báo này.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span><span class="sxs-lookup"><span data-stu-id="e5fab-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="e5fab-104">Để mở Trung tâm Bảo & Tuân thủ, hãy đi tới [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="e5fab-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="e5fab-105">Để mở trực tiếp trang Cách ly, hãy đi tới [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="e5fab-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="e5fab-106">Bạn có thể tìm kiếm theo các giá trị sau:</span><span class="sxs-lookup"><span data-stu-id="e5fab-106">You can search by the following values:</span></span>  

- <span data-ttu-id="e5fab-107">**ID Thư:** Mã định danh duy nhất toàn cầu của thư.</span><span class="sxs-lookup"><span data-stu-id="e5fab-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="e5fab-108">Nếu bạn chọn một thư trong danh sách, giá  **trị ID**  Thông báo sẽ xuất hiện  **trong**  ngăn cửa sổ bật lên Chi tiết xuất hiện.</span><span class="sxs-lookup"><span data-stu-id="e5fab-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="e5fab-109">Người quản trị có thể dùng [công cụ tìm thư](/microsoft-365/security/office-365-security/message-trace-scc) để tìm thư và các giá trị ID Thư tương ứng của chúng.</span><span class="sxs-lookup"><span data-stu-id="e5fab-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="e5fab-110">**Địa chỉ email người gửi:** Địa chỉ email của một người gửi đơn lẻ.</span><span class="sxs-lookup"><span data-stu-id="e5fab-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="e5fab-111">**Địa chỉ email người** nhận: Địa chỉ email của một người nhận duy nhất.</span><span class="sxs-lookup"><span data-stu-id="e5fab-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="e5fab-112">**Chủ** đề: Sử dụng toàn bộ chủ đề của thư.</span><span class="sxs-lookup"><span data-stu-id="e5fab-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="e5fab-113">Tìm kiếm không có chữ hoa/thường.</span><span class="sxs-lookup"><span data-stu-id="e5fab-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="e5fab-114">Sau khi bạn đã nhập các tiêu chí tìm kiếm, hãy bấm ![ Làm mới nút ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Làm** mới để lọc kết quả.</span><span class="sxs-lookup"><span data-stu-id="e5fab-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="e5fab-115">Lệnh ghép ngắn mà bạn dùng để xem và quản lý thư và tệp trong cách ly là:</span><span class="sxs-lookup"><span data-stu-id="e5fab-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="e5fab-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e5fab-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="e5fab-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e5fab-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="e5fab-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e5fab-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="e5fab-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Lưu ý rằng lệnh ghép ngắn này chỉ dành cho thư, không phải tệp phần mềm xấu từ Bộ bảo vệ Microsoft cho Office 365 cho SharePoint Online, OneDrive for Business hoặc Teams.</span><span class="sxs-lookup"><span data-stu-id="e5fab-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="e5fab-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="e5fab-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)