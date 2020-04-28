---
title: Sử dụng DLP trong quy tắc truyền tải
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915300"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="f84d0-102">Sử dụng DLP trong quy tắc truyền tải</span><span class="sxs-lookup"><span data-stu-id="f84d0-102">Using DLP in transport rules</span></span>

<span data-ttu-id="f84d0-103">Để tích hợp ngăn mất dữ liệu (DLP) vào một phương tiện hiện có, hãy sử dụng điều kiện "**Nếu thư chứa... Thông tin nhạy cảm**"trong cài đặt quy tắc truyền tải.</span><span class="sxs-lookup"><span data-stu-id="f84d0-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="f84d0-104">**Để biết thêm chi tiết, xem:**</span><span class="sxs-lookup"><span data-stu-id="f84d0-104">**For more details, see:**</span></span>

- <span data-ttu-id="f84d0-105">Các loại thông tin nhạy cảm DLP tích hợp trong các quy tắc truyền tải: [tích hợp các quy tắc thông tin nhạy cảm](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="f84d0-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="f84d0-106">Bạn cũng có thể kiểm tra quy tắc có hoặc không có kiểm tra chính sách bằng cách sử dụng chế độ kiểm tra trên quy tắc.</span><span class="sxs-lookup"><span data-stu-id="f84d0-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="f84d0-107">Bạn nên đợi 30 phút sau khi tạo quy tắc trước khi thử nghiệm nó.</span><span class="sxs-lookup"><span data-stu-id="f84d0-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="f84d0-108">Xem [kiểm tra dòng thư/quy tắc truyền tải](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="f84d0-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="f84d0-109">**Lưu ý**: nếu bạn đang cố gắng thực hiện một chính sách DLP mới với truyền tải quy tắc EAC, sử dụng [chính sách DLP bảo mật và tuân thủ trung tâm](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) thay thế.</span><span class="sxs-lookup"><span data-stu-id="f84d0-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
