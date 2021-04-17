---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821433"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="892ec-102">Khắc phục các sự cố chuyển phát email cho mã lỗi 5.7.23</span><span class="sxs-lookup"><span data-stu-id="892ec-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="892ec-103">Xác minh bản ghi SPF DNS cho tên miền của bạn tại một trình kiểm tra bản ghi SPF hoặc DNS công khai trên web.</span><span class="sxs-lookup"><span data-stu-id="892ec-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="892ec-104">Xác minh rằng thông báo gửi đi không được xác định là thư rác theo Microsoft và định tuyến thông qua [Hồ bơi chuyển giao rủi ro cao](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="892ec-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="892ec-105">Thư trong hồ bơi chuyển phát cao rủi ro sẽ không vượt qua kiểm tra SPF và do đó sẽ không được chấp nhận bởi tổ chức email đích.</span><span class="sxs-lookup"><span data-stu-id="892ec-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="892ec-106">Nếu sự cố vẫn tiếp diễn, bạn có thể cần liên hệ với người quản trị máy chủ thư mà bạn đang tìm cách gửi email.</span><span class="sxs-lookup"><span data-stu-id="892ec-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="892ec-107">Hãy lưu ý đến lỗi bên ngoài chi tiết sẵn dùng trong thư bị trả lại.</span><span class="sxs-lookup"><span data-stu-id="892ec-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="892ec-108">Hỗ trợ của Microsoft có thể không thể hỗ trợ thêm nữa.</span><span class="sxs-lookup"><span data-stu-id="892ec-108">Microsoft support may not be able to assist further.</span></span>
