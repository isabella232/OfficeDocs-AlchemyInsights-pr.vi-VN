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
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="d3ccc-102">Bật kiểm tra hộp thư</span><span class="sxs-lookup"><span data-stu-id="d3ccc-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="d3ccc-103">Để bật tính năng kiểm tra hộp thư cho một người dùng duy nhất hoặc toàn bộ tổ chức, hãy chạy các lệnh ghép ngắn sau đây từ Remote PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d3ccc-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="d3ccc-104">**Người dùng**: Set-Mailbox-Identity "Jane Dow"-AuditEnabled $True</span><span class="sxs-lookup"><span data-stu-id="d3ccc-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="d3ccc-105">**Tổ chức**: Get-Mailbox-ResultSize không giới hạn-Filter {RecipientTypeDetails-EQ "usermailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="d3ccc-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="d3ccc-106">Để tìm hiểu thêm, hãy xem [quản lý kiểm tra hộp thư](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="d3ccc-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>