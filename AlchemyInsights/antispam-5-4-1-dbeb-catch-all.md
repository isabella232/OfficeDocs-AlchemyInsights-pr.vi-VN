---
title: AntiSpam 5.4.1 DBEB Catch-tất cả
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4a56cfe74d8940e53a316d3bcc3809e8666c2e37
ms.sourcegitcommit: a8945ab0008f138b2992175b0640e78a505d29e1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37964377"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="ab1c7-102">Khắc phục sự cố phân phối cho mã lỗi 550 5.4.1 truy cập từ chối chuyển tiếp</span><span class="sxs-lookup"><span data-stu-id="ab1c7-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="ab1c7-103">Sự cố này xảy ra khi [kiểm tra xem địa chỉ email có hợp lệ để ngăn chặn bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) khi nhập mạng Office 365.</span><span class="sxs-lookup"><span data-stu-id="ab1c7-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Office 365 network.</span></span> <span data-ttu-id="ab1c7-104">Hãy thử các mục sau:</span><span class="sxs-lookup"><span data-stu-id="ab1c7-104">Try the following:</span></span>

1. <span data-ttu-id="ab1c7-105">Xác định xem sự cố dành riêng cho toàn bộ miền hoặc địa chỉ email duy nhất:</span><span class="sxs-lookup"><span data-stu-id="ab1c7-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="ab1c7-106">Toàn bộ miền: đôi khi miền cần được đồng bộ hoá; thử [đặt miền sang nội bộ và sau đó trở lại uỷ quyền](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="ab1c7-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
     - <span data-ttu-id="ab1c7-107">Địa chỉ email đơn: đôi khi địa chỉ cần được đồng bộ hoá; thay đổi địa chỉ proxy SMTP và sau đó thay đổi nó trở lại có thể giúp.</span><span class="sxs-lookup"><span data-stu-id="ab1c7-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="ab1c7-108">Xác định xem sự cố cụ thể cho một nhóm hoặc thư mục công cộng.</span><span class="sxs-lookup"><span data-stu-id="ab1c7-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="ab1c7-109">Đối với một số loại đối tượng, các đối tượng có thể cần phải được tạo theo cách thủ công trong Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ab1c7-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="ab1c7-110">Nếu bạn cần thêm sự giúp đỡ, vui lòng mở một vé hỗ trợ và chỉ định phạm vi của vấn đề (includidng loại đối tượng bạn đang gửi đến) để chúng tôi có thể hỗ trợ bạn tốt hơn.</span><span class="sxs-lookup"><span data-stu-id="ab1c7-110">If you need additional help, please open a support ticket and specify the scope of the issue (includidng the type of object you're sending to) so we can assist you better.</span></span>