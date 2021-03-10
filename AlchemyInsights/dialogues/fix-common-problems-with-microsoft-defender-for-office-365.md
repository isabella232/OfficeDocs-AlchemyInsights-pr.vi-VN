---
title: Khắc phục các sự cố phổ biến với Microsoft Defender cho Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 05fa518ece7ea40fd7b4cea57115d9cd60370b01
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695633"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a><span data-ttu-id="692a2-102">Khắc phục các sự cố phổ biến với Microsoft Defender cho Office 365</span><span class="sxs-lookup"><span data-stu-id="692a2-102">Fix common problems with Microsoft Defender for Office 365</span></span>

<span data-ttu-id="692a2-103">Dưới đây là một số giải pháp cho các vấn đề thường gặp với Microsoft Defender cho Office 365:</span><span class="sxs-lookup"><span data-stu-id="692a2-103">Here are some solutions to common problems with Microsoft Defender for Office 365:</span></span>

- <span data-ttu-id="692a2-104">Độ **trễ thư:** Nếu bạn đang gặp sự cố khi chuyển phát thư bị trì hoãn, bạn sẽ muốn sử dụng các tùy chọn chuyển phát **động** trong chính sách tệp đính kèm an toàn của bạn.</span><span class="sxs-lookup"><span data-stu-id="692a2-104">**Message delay:** If you're experiencing issues where message delivery is delayed, you'll want to use the **Dynamic Delivery** options within your Safe Attachments policy.</span></span> <span data-ttu-id="692a2-105">Để tìm hiểu thêm, hãy xem [phân phát động trong chính sách tệp đính kèm an toàn](https://go.microsoft.com/fwlink/?linkid=2094106).</span><span class="sxs-lookup"><span data-stu-id="692a2-105">To learn more, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2094106).</span></span>
- <span data-ttu-id="692a2-106">**Báo cáo kết quả dương tính false hoặc âm:** Báo cáo thư cho Microsoft bằng cách sử dụng liên kết này: [cổng thông tin phản hồi của Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2092835).</span><span class="sxs-lookup"><span data-stu-id="692a2-106">**Report false positive or negative results:** Report the message to Microsoft using this link: [Microsoft Defender Response Portal](https://go.microsoft.com/fwlink/?linkid=2092835).</span></span>
- <span data-ttu-id="692a2-107">**Cho phép bảo vệ liên kết an toàn:**</span><span class="sxs-lookup"><span data-stu-id="692a2-107">**Enable Safe Link protection:**</span></span>
    1. <span data-ttu-id="692a2-108">Đăng nhập vào [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="692a2-108">Sign in to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
    2. <span data-ttu-id="692a2-109">Đi đến   >    >  **nối kết an toàn** chính sách quản lý mối đe dọa.</span><span class="sxs-lookup"><span data-stu-id="692a2-109">Go to **Threat Management** > **Policy** > **Safe Links.**</span></span>
    3. <span data-ttu-id="692a2-110">Bên dưới **chính sách áp dụng cho những người nhận cụ thể**, hãy mở chính sách được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="692a2-110">Under **Policies that apply to specific recipients**, open the policy configured.</span></span>
    4. <span data-ttu-id="692a2-111">Bên dưới **thiết đặt**, hãy chọn **áp dụng nối kết an toàn cho thư được gửi trong tổ chức**.</span><span class="sxs-lookup"><span data-stu-id="692a2-111">Under **Settings**, select **Apply safe links to messages sent within the organization**.</span></span>
