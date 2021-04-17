---
title: Khắc phục sự kiện từ email
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834861"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="61bb0-102">Khắc phục sự kiện từ email</span><span class="sxs-lookup"><span data-stu-id="61bb0-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="61bb0-103">Xác nhận tính năng được kích hoạt cho hộp thư: **Get-Eventsfroconfiguration-danh <mailbox> tính**</span><span class="sxs-lookup"><span data-stu-id="61bb0-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="61bb0-104">Sau đó, hãy xem mục các sự kiện ' từ xuất Nhật ký của email **-MailboxDiagnosticLogs <mailbox> -khung hồ sơ thành phần**</span><span class="sxs-lookup"><span data-stu-id="61bb0-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="61bb0-105">Trong Nhật ký ' các sự kiện từ email, hãy tìm InternetMessageId khớp với mục đó trong hộp thư.</span><span class="sxs-lookup"><span data-stu-id="61bb0-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="61bb0-106">Trustđiểm sẽ xác định nếu mục được thêm vào hay không.</span><span class="sxs-lookup"><span data-stu-id="61bb0-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="61bb0-107">Sự kiện sẽ chỉ được thêm vào nếu Trust= = "tin cậy".</span><span class="sxs-lookup"><span data-stu-id="61bb0-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="61bb0-108">Trustđiểm được xác định bởi SPF, các thuộc tính Mkim hoặc Nhmarc, nằm trong phần đầu thư.</span><span class="sxs-lookup"><span data-stu-id="61bb0-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="61bb0-109">Để xem các thuộc tính sau:</span><span class="sxs-lookup"><span data-stu-id="61bb0-109">To view these properties:</span></span>

<span data-ttu-id="61bb0-110">**Outlook trên máy tính**</span><span class="sxs-lookup"><span data-stu-id="61bb0-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="61bb0-111">Mở mục</span><span class="sxs-lookup"><span data-stu-id="61bb0-111">Open the item</span></span>
- <span data-ttu-id="61bb0-112">Thuộc tính > tệp-> tiêu đề Internet</span><span class="sxs-lookup"><span data-stu-id="61bb0-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="61bb0-113">hay</span><span class="sxs-lookup"><span data-stu-id="61bb0-113">or</span></span>

<span data-ttu-id="61bb0-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="61bb0-114">**MFCMapi**</span></span>

- <span data-ttu-id="61bb0-115">Dẫn hướng đến mục trong hộp thư đến</span><span class="sxs-lookup"><span data-stu-id="61bb0-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="61bb0-116">Tìm PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="61bb0-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="61bb0-117">Những thuộc tính này được xác định và ghi lại trong quá trình vận chuyển và định tuyến.</span><span class="sxs-lookup"><span data-stu-id="61bb0-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="61bb0-118">Để khắc phục sự cố thêm, bạn có thể cần phải theo dõi với hỗ trợ truyền tải về các lỗi trong SPF, MKIM và. hoặc TMARC.</span><span class="sxs-lookup"><span data-stu-id="61bb0-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>