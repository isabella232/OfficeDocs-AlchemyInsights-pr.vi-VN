---
title: Bật tính năng kiểm tra hộp thư
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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058060"
---
# <a name="turn-on-mailbox-auditing"></a>Bật tính năng kiểm tra hộp thư

Để bật tính năng kiểm tra hộp thư cho một người dùng hoặc toàn bộ tổ chức, hãy chạy lệnh ghép ngắn sau từ PowerShell Từ xa:

- **Người dùng đơn** lẻ : Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **Tổ** chức : Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Để tìm hiểu thêm, xem mục [Quản lý kiểm tra hộp thư](https://go.microsoft.com/fwlink/?linkid=2103668).