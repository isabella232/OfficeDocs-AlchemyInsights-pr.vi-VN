---
title: Bạn cần trợ giúp với giới hạn gửi email?
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
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702385"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="4b6b7-102">Bạn cần trợ giúp với giới hạn gửi email?</span><span class="sxs-lookup"><span data-stu-id="4b6b7-102">Need help with email sending limits?</span></span>

<span data-ttu-id="4b6b7-103">Dưới đây là **giới hạn gửi theo thiết kế** được áp thi trong dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="4b6b7-104">Thông tin thêm về các giới hạn này là tài liệu [ở đây](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="4b6b7-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="4b6b7-105">Để ngăn không cho việc chuyển phát thư hàng loạt không mong muốn, chúng tôi áp dụng **giới hạn tỷ lệ người nhận trên toàn người dùng cho tất cả các thư đi và nội bộ**.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="4b6b7-106">Trên tất cả các SKUs, giới hạn này là **10.000 người nhận mỗi ngày**.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="4b6b7-107">Khách hàng cần gửi email thương mại hàng loạt hợp pháp (ví dụ, bản tin khách hàng) nên sử dụng các nhà cung cấp bên thứ ba chuyên về các dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="4b6b7-108">**Lưu ý**: khi đã đạt đến giới hạn số lượng người nhận, không thể gửi thư từ hộp thư cho đến khi số người nhận đã gửi thư trong vòng 24 giờ qua dưới giới hạn.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="4b6b7-109">Người dùng sẽ không thể gửi thư cho đến khi đó.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="4b6b7-110">Giới hạn tỷ suất thư của **30 thư mỗi phút** được áp dụng trên tất cả các SKUs.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="4b6b7-111">Điều này sẽ xác định có bao nhiêu thư người dùng có thể gửi từ tài khoản Exchange Online của họ trong một khoảng thời gian đã xác định.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="4b6b7-112">**Số lượng người nhận tối đa được phép trong các trường đến, CC và Bcc** cho một email đơn lẻ, trên tất cả các **người nhận 1000**.</span><span class="sxs-lookup"><span data-stu-id="4b6b7-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="4b6b7-113">Để tùy chỉnh giới hạn này, hãy đến [đây](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="4b6b7-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
