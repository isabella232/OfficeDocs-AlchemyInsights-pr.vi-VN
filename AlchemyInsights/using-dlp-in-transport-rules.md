---
title: Sử dụng khoảng cách trong quy tắc truyền dẫn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 00ea5e67d1277e4a2a73d616b1f90d6e4bc5b54f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773185"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="3ae7f-102">Sử dụng khoảng cách trong quy tắc truyền dẫn</span><span class="sxs-lookup"><span data-stu-id="3ae7f-102">Using DLP in transport rules</span></span>

<span data-ttu-id="3ae7f-103">Để tích hợp phòng chống mất dữ liệu (đã chuyển) vào một phương tiện truyền thông hiện có, hãy sử dụng điều kiện "**Nếu thư chứa... Thông tin nhạy cảm**"trong thiết đặt quy tắc truyền dẫn.</span><span class="sxs-lookup"><span data-stu-id="3ae7f-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="3ae7f-104">**Để biết thêm chi tiết, hãy xem:**</span><span class="sxs-lookup"><span data-stu-id="3ae7f-104">**For more details, see:**</span></span>

- <span data-ttu-id="3ae7f-105">Tích hợp các loại thông tin nhạy cảm trong quy tắc truyền dẫn: [tích hợp quy tắc thông tin nhạy cảm](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="3ae7f-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="3ae7f-106">Bạn cũng có thể kiểm tra quy tắc có hoặc không có kiểm tra chính sách bằng cách sử dụng chế độ kiểm tra trên quy tắc.</span><span class="sxs-lookup"><span data-stu-id="3ae7f-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="3ae7f-107">Bạn nên đợi 30 phút sau khi tạo quy tắc trước khi thử nghiệm.</span><span class="sxs-lookup"><span data-stu-id="3ae7f-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="3ae7f-108">Xem [kiểm tra quy tắc dòng thư/truyền](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules) dẫn</span><span class="sxs-lookup"><span data-stu-id="3ae7f-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="3ae7f-109">**Lưu ý**: nếu bạn đang cố gắng thực hiện chính sách có dạng mới với quy tắc truyền tải trong EAC, hãy sử dụng chính sách đã thu được [trong Trung tâm bảo mật và tuân thủ](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) .</span><span class="sxs-lookup"><span data-stu-id="3ae7f-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
