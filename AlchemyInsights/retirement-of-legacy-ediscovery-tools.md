---
title: Hưu trí của công cụ eDiscovery kế thừa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727805"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="8d9c6-102">Hưu trí của công cụ eDiscovery kế thừa</span><span class="sxs-lookup"><span data-stu-id="8d9c6-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="8d9c6-103">Là kết quả của chức năng khám phá điện tử mới và được cải tiến trong Trung tâm tuân thủ Microsoft 365, các công cụ và lệnh ghép ngắn sau đây được thiết kế lại sau đó sẽ được ngừng hoạt động trong những tháng sắp tới:</span><span class="sxs-lookup"><span data-stu-id="8d9c6-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="8d9c6-104">[Khám phá điện tử tại chỗ](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) và [tại chỗ giữ](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) trong Trung tâm quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="8d9c6-105">Các lệnh ghép ngắn Exchange Online PowerShell hỗ trợ khám phá điện tử tại chỗ và giữ tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="8d9c6-106">(Các lệnh ghép ngắn này được xác định chung là lệnh ghép ngắn \*-MailboxSearch.) Điều này bao gồm các lệnh ghép ngắn sau đây:</span><span class="sxs-lookup"><span data-stu-id="8d9c6-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="8d9c6-107">Mới-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8d9c6-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="8d9c6-108">Khởi động-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8d9c6-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="8d9c6-109">Ngăn chặn-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8d9c6-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="8d9c6-110">Thiết đặt-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="8d9c6-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="8d9c6-111">Lệnh ghép ngắn [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) trong Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="8d9c6-112">Các thao tác sau trong API Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="8d9c6-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="8d9c6-113">Tìm kiếm hộp thư</span><span class="sxs-lookup"><span data-stu-id="8d9c6-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="8d9c6-114">Setholdonhộp thư</span><span class="sxs-lookup"><span data-stu-id="8d9c6-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="8d9c6-115">Getholdonhộp thư</span><span class="sxs-lookup"><span data-stu-id="8d9c6-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="8d9c6-116">Nâng cao eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="8d9c6-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="8d9c6-117">**Đường thời gian cho quỹ hưu trí**:</span><span class="sxs-lookup"><span data-stu-id="8d9c6-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="8d9c6-118">**Ngày 1 tháng 7, 2020** Bạn không còn có thể tạo các tìm kiếm mới và giữ, nhưng bạn có thể chạy, chỉnh sửa và xóa bỏ các tìm kiếm hiện có theo rủi ro của riêng bạn.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="8d9c6-119">Hỗ trợ của Microsoft không còn hỗ trợ trong khám phá điện tử tại chỗ & giữ trong EAC.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="8d9c6-120">**Ngày 1 tháng 10, 2020** Khám phá điện tử tại chỗ & giữ chức năng trong EAC sẽ được đặt ở chế độ chỉ đọc, vì vậy bạn chỉ có thể loại bỏ các tìm kiếm hiện có và giữ.</span><span class="sxs-lookup"><span data-stu-id="8d9c6-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="8d9c6-121">**Để biết thêm thông tin, hãy xem**:</span><span class="sxs-lookup"><span data-stu-id="8d9c6-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="8d9c6-122">Di chuyển các tìm kiếm khám phá điện tử và giữ lại Trung tâm tuân thủ Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8d9c6-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="8d9c6-123">Hưu trí của công cụ eDiscovery kế thừa</span><span class="sxs-lookup"><span data-stu-id="8d9c6-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="8d9c6-124">Các câu hỏi thường gặp về khám phá điện tử tại chỗ và giữ tại chỗ</span><span class="sxs-lookup"><span data-stu-id="8d9c6-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



