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
# <a name="your-archive-mailbox-is-almost-full"></a>Hộp thư lưu trữ của bạn gần như đầy đủ

Nếu người dùng nhận được cảnh báo; **Hộp thư lưu trữ của bạn gần như đầy đủ**, hoặc bạn cần tăng kích cỡ hộp thư lưu trữ của họ, dưới đây là một số Mẹo:

1. Nếu người dùng được gán một gói Exchange Online 1, nâng cấp lên **Exchange Online Plan 2** giấy phép để tăng kích cỡ từ 50 GB đến 100gb.
1. Nếu người dùng đã được gán một trong những thao tác sau đây: **Exchange Online Plan 2** hoặc gói Exchange Online 1 với phần bổ trợ lưu trữ Exchange Online, hãy làm theo các bước dưới đây để bật tự động mở rộng lưu trữ:.
 
    1. [Kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Chạy lệnh ghép ngắn sau đây cho người dùng:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Chạy lệnh ghép ngắn sau đây để xác nhận đã được kích hoạt cho người dùng:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Để biết thêm thông tin, hãy xem:

- [ Bật lưu trữ không giới hạn-trợ giúp người quản trị-Microsoft 365 tuân thủ | Tài liệu Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Giới hạn Exchange Online-mô tả Dịch vụ | Tài liệu Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nâng cấp lên kế hoạch kinh doanh khác | Tài liệu Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

