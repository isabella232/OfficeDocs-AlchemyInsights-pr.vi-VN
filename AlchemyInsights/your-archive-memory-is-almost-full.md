---
title: Hộp thư lưu trữ của bạn sắp đầy
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046774"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Hộp thư lưu trữ của bạn sắp đầy

Nếu người dùng nhận được cảnh báo; **Hộp thư lưu trữ của bạn gần đầy** hoặc bạn cần tăng kích cỡ hộp thư lưu trữ của họ, dưới đây là một số mẹo:

1. Nếu người dùng được gán giấy phép Exchange Online Plan 1, hãy nâng cấp lên **Exchange Online Plan 2** để tăng kích cỡ từ 50 GB lên 100GB.
1. Nếu người dùng đã được gán một trong những thông tin sau: **Exchange Online Plan 2** hoặc Exchange Online Plan 1 với phần bổ trợ Exchange Online Archiving, hãy sử dụng các bước dưới đây để bật tính năng lưu trữ Bung rộng Tự động:.
 
    1. [Kết nối đổi Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Chạy commandlet sau đây cho người dùng:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Chạy commandlet sau đây để xác nhận rằng lệnh được bật cho người dùng:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Để biết thêm thông tin, hãy xem:

- [Cho phép lưu trữ không giới hạn - Trợ giúp Người quản trị - Microsoft 365 tuân | Tài liệu Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online hạn - Mô tả Dịch vụ | Tài liệu Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nâng cấp lên gói doanh nghiệp khác | Tài liệu Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

