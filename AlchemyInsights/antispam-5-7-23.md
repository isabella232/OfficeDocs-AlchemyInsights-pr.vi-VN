---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506465"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="a4184-102">Khắc phục sự cố gửi email cho mã lỗi 5.7.23</span><span class="sxs-lookup"><span data-stu-id="a4184-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="a4184-103">Xác minh bản ghi SPF DNS cho miền của bạn tại một công khai có SPF hoặc kiểm tra bản ghi DNS trên web.</span><span class="sxs-lookup"><span data-stu-id="a4184-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="a4184-104">Xác minh rằng thư đi không được xác định là thư rác của Microsoft và chuyển qua vùng [phân phối rủi ro cao](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="a4184-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="a4184-105">Thư trong vùng phân phối rủi ro cao sẽ không vượt qua kiểm tra SPF và do đó sẽ không được chấp nhận bởi tổ chức email đích.</span><span class="sxs-lookup"><span data-stu-id="a4184-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="a4184-106">Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với quản trị viên của máy chủ thư mà bạn đang cố gắng gửi email.</span><span class="sxs-lookup"><span data-stu-id="a4184-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="a4184-107">Hãy lưu ý các lỗi bên ngoài chi tiết có sẵn trong thư trả lại.</span><span class="sxs-lookup"><span data-stu-id="a4184-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="a4184-108">Hỗ trợ của Microsoft không thể hỗ trợ thêm.</span><span class="sxs-lookup"><span data-stu-id="a4184-108">Microsoft support may not be able to assist further.</span></span>
