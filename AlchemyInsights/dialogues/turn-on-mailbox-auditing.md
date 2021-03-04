---
title: Bật kiểm tra hộp thư
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430248"
---
# <a name="turn-on-mailbox-auditing"></a>Bật kiểm tra hộp thư

Để bật tính năng kiểm tra hộp thư cho một người dùng duy nhất hoặc toàn bộ tổ chức, hãy chạy các lệnh ghép ngắn sau đây từ Remote PowerShell:

- **Người dùng**: Set-Mailbox-Identity "Jane Dow"-AuditEnabled $True
- **Tổ chức**: Get-Mailbox-ResultSize không giới hạn-Filter {RecipientTypeDetails-EQ "usermailbox"} | Set-Mailbox-AuditEnabled $true

Để tìm hiểu thêm, hãy xem [quản lý kiểm tra hộp thư](https://go.microsoft.com/fwlink/?linkid=2103668).