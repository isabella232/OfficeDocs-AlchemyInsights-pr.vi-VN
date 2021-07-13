---
title: Nhóm chuyển tiếp đi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381868"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="9ea18-102">Nhóm chuyển tiếp đi</span><span class="sxs-lookup"><span data-stu-id="9ea18-102">Outbound relay pool</span></span>

<span data-ttu-id="9ea18-103">Microsoft đang thực hiện một số thay đổi đối với cấu hình để chuyển tiếp hoặc chuyển tiếp email thông qua Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ea18-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="9ea18-104">Thư trong một số kịch bản nhất định được chuyển tiếp hoặc chuyển tiếp thông qua Microsoft 365 dụng một nhóm chuyển tiếp đặc biệt.</span><span class="sxs-lookup"><span data-stu-id="9ea18-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="9ea18-105">Thư được gửi bằng cách dùng nhóm chuyển tiếp có thể dẫn đến thư mục thư rác của người nhận.</span><span class="sxs-lookup"><span data-stu-id="9ea18-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="9ea18-106">Để biết thêm thông tin, hãy [xem Nhóm chuyển phát đi](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="9ea18-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="9ea18-107">Để tránh kịch bản sử dụng nhóm chuyển tiếp, hãy đảm bảo rằng các thư chuyển tiếp/chuyển tiếp đáp ứng một trong các tiêu chí sau đây:</span><span class="sxs-lookup"><span data-stu-id="9ea18-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="9ea18-108">Người gửi đi là tên miền được chấp nhận của đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="9ea18-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="9ea18-109">Khung Chính sách Người gửi (SPF) đi qua khi thư đến và Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ea18-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="9ea18-110">Thư được Xác định bởi DomainKeys (DKIM) trên miền người gửi P2 đi qua khi thư đến Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9ea18-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="9ea18-111">Những thư đáp ứng các tiêu chí trên sẽ không được chuyển tiếp qua nhóm chuyển tiếp.</span><span class="sxs-lookup"><span data-stu-id="9ea18-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="9ea18-112">Nếu bản ghi MX cho tên miền của bạn được trỏ tới một máy chủ bên thứ ba hoặc tại chỗ, hãy sử dụng bộ lọc nâng cao để đảm bảo xác thực SPF chính xác cho email đến và tránh gửi email qua vùng chuyển tiếp.</span><span class="sxs-lookup"><span data-stu-id="9ea18-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="9ea18-113">**Làm thế nào để chúng tôi biết chúng tôi bị ảnh hưởng bởi nhóm chuyển tiếp?**</span><span class="sxs-lookup"><span data-stu-id="9ea18-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="9ea18-114">Nếu email chuyển tiếp hoặc chuyển tiếp sử dụng một trong các tiêu chí ở trên, thư sẽ không được chuyển tiếp thông qua nhóm chuyển tiếp.</span><span class="sxs-lookup"><span data-stu-id="9ea18-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="9ea18-115">Tuy nhiên, nếu thư được gửi thông qua một nhóm chuyển tiếp, IP của máy chủ thư đi nằm trong phạm vi 40.95.0.0/16 và tên máy chủ thư đi chứa **rly** trong tên.</span><span class="sxs-lookup"><span data-stu-id="9ea18-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

