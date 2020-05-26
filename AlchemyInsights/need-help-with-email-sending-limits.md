---
title: Bạn cần trợ giúp với giới hạn gửi email?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358363"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="b8300-102">Bạn cần trợ giúp với giới hạn gửi email?</span><span class="sxs-lookup"><span data-stu-id="b8300-102">Need help with email sending limits?</span></span>

<span data-ttu-id="b8300-103">Dưới đây là **giới hạn gửi bằng thiết kế** thi hành trong dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="b8300-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="b8300-104">Thông tin thêm về các giới hạn này được ghi lại [ở đây](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="b8300-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="b8300-105">Để ngăn việc phân phối các thư hàng loạt không mong muốn, chúng tôi áp dụng giới hạn tỷ lệ người nhận cho mỗi người dùng cho **tất cả các thư bên ngoài và nội bộ**.</span><span class="sxs-lookup"><span data-stu-id="b8300-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="b8300-106">Trên tất cả các SKU, giới hạn này là **10.000 người nhận mỗi ngày**.</span><span class="sxs-lookup"><span data-stu-id="b8300-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="b8300-107">Khách hàng cần gửi email thương mại hàng loạt hợp pháp (ví dụ: bản tin khách hàng) nên sử dụng các nhà cung cấp bên thứ ba chuyên về các dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="b8300-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="b8300-108">**Lưu ý**: khi đạt đến giới hạn tỷ lệ người nhận, thư không được gửi từ hộp thư cho đến khi số lượng người nhận được gửi thư trong 24 giờ qua giảm xuống dưới giới hạn.</span><span class="sxs-lookup"><span data-stu-id="b8300-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="b8300-109">Người dùng sẽ không thể gửi thư đến điểm đó.</span><span class="sxs-lookup"><span data-stu-id="b8300-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="b8300-110">Giới hạn tốc độ tin nhắn của **30 tin nhắn mỗi phút** được áp dụng trên tất cả SKU.</span><span class="sxs-lookup"><span data-stu-id="b8300-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="b8300-111">Điều này xác định có bao nhiêu thư người dùng có thể gửi từ tài khoản Exchange Online của họ trong một khoảng thời gian xác định.</span><span class="sxs-lookup"><span data-stu-id="b8300-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="b8300-112">**Số lượng người nhận tối đa được phép trong các trường đến, CC và Bcc** cho một thư email duy nhất, trên tất cả SKU, là **1000 người nhận**.</span><span class="sxs-lookup"><span data-stu-id="b8300-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="b8300-113">Để tùy chỉnh giới hạn này, hãy vào [đây](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="b8300-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
