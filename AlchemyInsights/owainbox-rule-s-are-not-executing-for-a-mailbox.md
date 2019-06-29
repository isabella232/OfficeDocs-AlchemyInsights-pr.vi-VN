---
title: 1332 OWA - hộp thư đến rule(s) không thực hiện cho một hộp thư
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360939"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5b5c2-102">Quy tắc hộp thư đến không hoạt động như mong đợi</span><span class="sxs-lookup"><span data-stu-id="5b5c2-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5b5c2-103">Xác minh các cài đặt sau:</span><span class="sxs-lookup"><span data-stu-id="5b5c2-103">Verify the following settings:</span></span>

- <span data-ttu-id="5b5c2-104">Một tin nhắn có thể được chuyển hướng, chuyển tiếp, hoặc trả lời: tự động dựa trên các quy tắc hộp thư đến chỉ một lần.</span><span class="sxs-lookup"><span data-stu-id="5b5c2-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5b5c2-105">Một quy tắc chuyển hướng (một quy tắc hộp thư đến hoặc thư quy luật dòng chảy, cũng được biết đến như là một quy tắc truyền tải) có thể thêm tối đa mười chuyển người nhận thư.</span><span class="sxs-lookup"><span data-stu-id="5b5c2-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5b5c2-106">Để biết thêm chi tiết, hãy xem [tạp chí, giao thông vận tải, và hộp thư đến nguyên tắc giới hạn](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="5b5c2-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5b5c2-107">Quy tắc hộp thư đến không làm việc trên hộp thư ghi nhật ký khác.</span><span class="sxs-lookup"><span data-stu-id="5b5c2-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5b5c2-108">Để biết thêm chi tiết về hộp thư ghi nhật ký khác, hãy xem [hộp thư ghi nhật ký thay thế](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="5b5c2-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5b5c2-109">Để khắc phục những vấn đề này, hãy xem [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="5b5c2-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5b5c2-110">Nếu các vấn đề trước đó không áp dụng, hãy chạy báo cáo chuẩn đoán quy tắc hộp thư đến trước khi bạn leo thang các vấn đề cho Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="5b5c2-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5b5c2-111">Mở hộp thư trong Outlook trên web và nhấp vào **cài đặt** \> **tùy chọn** \> **tổ chức email** \> **quy tắc hộp thư đến**.</span><span class="sxs-lookup"><span data-stu-id="5b5c2-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="5b5c2-112">Ở dưới cùng của trang, nhấp vào **nếu quy tắc của bạn không làm việc bấm vào đây để tạo ra một báo cáo chuẩn đoán**.</span><span class="sxs-lookup"><span data-stu-id="5b5c2-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
