---
title: Hộp thư lưu trữ của bạn gần như đầy đủ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974669"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="4cf51-102">Hộp thư lưu trữ của bạn gần như đầy đủ</span><span class="sxs-lookup"><span data-stu-id="4cf51-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="4cf51-103">Nếu người dùng nhận được cảnh báo; **Hộp thư lưu trữ của bạn gần như đầy đủ**, hoặc bạn cần tăng kích cỡ hộp thư lưu trữ của họ, dưới đây là một số Mẹo:</span><span class="sxs-lookup"><span data-stu-id="4cf51-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="4cf51-104">Nếu người dùng được gán một gói Exchange Online 1, nâng cấp lên **Exchange Online Plan 2** giấy phép để tăng kích cỡ từ 50 GB đến 100gb.</span><span class="sxs-lookup"><span data-stu-id="4cf51-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="4cf51-105">Nếu người dùng đã được gán một trong những thao tác sau đây: **Exchange Online Plan 2** hoặc gói Exchange Online 1 với phần bổ trợ lưu trữ Exchange Online, hãy làm theo các bước dưới đây để bật tự động mở rộng lưu trữ:.</span><span class="sxs-lookup"><span data-stu-id="4cf51-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="4cf51-106">[Kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4cf51-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="4cf51-107">Chạy lệnh ghép ngắn sau đây cho người dùng:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="4cf51-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="4cf51-108">Chạy lệnh ghép ngắn sau đây để xác nhận đã được kích hoạt cho người dùng:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="4cf51-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="4cf51-109">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="4cf51-109">For more information see:</span></span>

- [<span data-ttu-id="4cf51-110"> Bật lưu trữ không giới hạn-trợ giúp người quản trị-Microsoft 365 tuân thủ | Tài liệu Microsoft</span><span class="sxs-lookup"><span data-stu-id="4cf51-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="4cf51-111">Giới hạn Exchange Online-mô tả Dịch vụ | Tài liệu Microsoft</span><span class="sxs-lookup"><span data-stu-id="4cf51-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="4cf51-112">Nâng cấp lên kế hoạch kinh doanh khác | Tài liệu Microsoft</span><span class="sxs-lookup"><span data-stu-id="4cf51-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

