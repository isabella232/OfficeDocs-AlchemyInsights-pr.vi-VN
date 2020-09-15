---
title: AntiSpam 5.4.1 \ Catch-tất cả
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
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717383"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="3b11f-102">Khắc phục các sự cố chuyển phát cho mã lỗi 550 5.4.1 Relay Access bị từ chối</span><span class="sxs-lookup"><span data-stu-id="3b11f-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="3b11f-103">Sự cố này xảy ra khi [kiểm tra để xem liệu một địa chỉ email có hiệu lực hợp lệ không để ngăn chặn](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) khi nhập mạng Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3b11f-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="3b11f-104">Hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="3b11f-104">Try the following:</span></span>

1. <span data-ttu-id="3b11f-105">Xác định xem vấn đề này là gì cụ thể đối với toàn bộ tên miền hoặc địa chỉ email duy nhất:</span><span class="sxs-lookup"><span data-stu-id="3b11f-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="3b11f-106">Toàn bộ tên miền: đôi khi tên miền cần được đồng bộ hóa; thử [đặt tên miền thành nội bộ và sau đó trở lại thẩm quyền](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="3b11f-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="3b11f-107">Địa chỉ email đơn: đôi khi địa chỉ cần được đồng bộ hóa; thay đổi địa chỉ proxy SMTP và sau đó thay đổi nó lại có thể trợ giúp.</span><span class="sxs-lookup"><span data-stu-id="3b11f-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="3b11f-108">Xác định xem vấn đề này là gì cụ thể đối với một nhóm hoặc thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="3b11f-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="3b11f-109">Đối với một số loại đối tượng, các đối tượng có thể cần được tạo theo cách thủ công trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3b11f-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="3b11f-110">Nếu bạn cần thêm trợ giúp, vui lòng mở một vé hỗ trợ và xác định phạm vi vấn đề (bao gồm loại đối tượng mà bạn đang gửi đến) để chúng tôi có thể hỗ trợ bạn tốt hơn.</span><span class="sxs-lookup"><span data-stu-id="3b11f-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>