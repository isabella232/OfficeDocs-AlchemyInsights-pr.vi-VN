---
title: Bảo vệ khỏi cuộc tấn công lùi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037184"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="8240d-102">Bảo vệ khỏi cuộc tấn công lùi</span><span class="sxs-lookup"><span data-stu-id="8240d-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="8240d-103">Backscatter là các báo cáo không chuyển phát (còn được gọi là thư bị trả lại), bạn sẽ nhận được những tin nhắn mà bạn không gửi.</span><span class="sxs-lookup"><span data-stu-id="8240d-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="8240d-104">Gửi thư rác giả mạo (spoof) **từ:** địa chỉ thư của họ, và họ thường dùng địa chỉ email thực để cho vay tin cậy vào thư của họ.</span><span class="sxs-lookup"><span data-stu-id="8240d-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="8240d-105">Vì vậy, khi gửi thư rác không chắc chắn gửi thư đến người nhận không tồn tại, máy chủ email đích sẽ bị lừa trở về thư không được gửi đi trong NDR đến người gửi giả mạo trong **từ:** address.</span><span class="sxs-lookup"><span data-stu-id="8240d-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="8240d-106">Có thể tìm thấy thông tin bổ sung trong [backscatter trong EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="8240d-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="8240d-107">**Bật tính năng bảo vệ chống phân tán**</span><span class="sxs-lookup"><span data-stu-id="8240d-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="8240d-108">Để cho phép bảo vệ lên dưới, hãy làm theo đường dẫn bên dưới.</span><span class="sxs-lookup"><span data-stu-id="8240d-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="8240d-109">**protection.office.com > quản lý mối đe dọa > chính sách > antispam > chọn chính sách bộ lọc thư rác và sửa chính sách > thuộc tính thư rác > đánh dấu là thư rác > NDR đã bật tiếng > đặt nó thành "bật"**</span><span class="sxs-lookup"><span data-stu-id="8240d-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="8240d-110">Nếu bạn tin rằng tài khoản đã bị xâm phạm, hãy xem những điều sau đây:</span><span class="sxs-lookup"><span data-stu-id="8240d-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="8240d-111">Trả lời tài khoản email bị xâm phạm</span><span class="sxs-lookup"><span data-stu-id="8240d-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="8240d-112">Loại bỏ người dùng bị chặn khỏi cổng thông tin người dùng bị hạn chế trong Office 365</span><span class="sxs-lookup"><span data-stu-id="8240d-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



