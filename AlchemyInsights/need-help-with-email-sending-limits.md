---
title: Bạn cần trợ giúp với giới hạn gửi email?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836301"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="cf194-102">Bạn cần trợ giúp với giới hạn gửi email?</span><span class="sxs-lookup"><span data-stu-id="cf194-102">Need help with email sending limits?</span></span>

<span data-ttu-id="cf194-103">Dưới đây là **giới hạn gửi theo thiết kế** được áp thi trong dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="cf194-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="cf194-104">Thông tin thêm về các giới hạn này là tài liệu [ở đây](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="cf194-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="cf194-105">Để ngăn không cho việc chuyển phát thư hàng loạt không mong muốn, chúng tôi áp dụng **giới hạn tỷ lệ người nhận trên toàn người dùng cho tất cả các thư đi và nội bộ**.</span><span class="sxs-lookup"><span data-stu-id="cf194-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="cf194-106">Trên tất cả các SKUs, giới hạn này là **10.000 người nhận mỗi ngày**.</span><span class="sxs-lookup"><span data-stu-id="cf194-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="cf194-107">Khách hàng cần gửi email thương mại hàng loạt hợp pháp (ví dụ, bản tin khách hàng) nên sử dụng các nhà cung cấp bên thứ ba chuyên về các dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="cf194-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="cf194-108">**Lưu ý**: khi đã đạt đến giới hạn số lượng người nhận, không thể gửi thư từ hộp thư cho đến khi số người nhận đã gửi thư trong vòng 24 giờ qua dưới giới hạn.</span><span class="sxs-lookup"><span data-stu-id="cf194-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="cf194-109">Người dùng sẽ không thể gửi thư cho đến khi đó.</span><span class="sxs-lookup"><span data-stu-id="cf194-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="cf194-110">Giới hạn tỷ suất thư của **30 thư mỗi phút** được áp dụng trên tất cả các SKUs.</span><span class="sxs-lookup"><span data-stu-id="cf194-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="cf194-111">Điều này sẽ xác định có bao nhiêu thư người dùng có thể gửi từ tài khoản Exchange Online của họ trong một khoảng thời gian đã xác định.</span><span class="sxs-lookup"><span data-stu-id="cf194-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="cf194-112">**Số lượng người nhận tối đa được phép trong các trường đến, CC và Bcc** cho một email đơn lẻ, trên tất cả các **người nhận 1000**.</span><span class="sxs-lookup"><span data-stu-id="cf194-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="cf194-113">Để tùy chỉnh giới hạn này, hãy đến [đây](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="cf194-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
