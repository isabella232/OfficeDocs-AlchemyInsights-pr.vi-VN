---
title: Bật kiểm tra hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506976"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="89b18-102">Bật kiểm tra hộp thư</span><span class="sxs-lookup"><span data-stu-id="89b18-102">Enable mailbox auditing</span></span>

<span data-ttu-id="89b18-103">Để kích hoạt hộp kiểm tra cho người dùng hoặc một tổ chức toàn bộ các lệnh ghép ngắn sau đây phải được chạy từ xa điện vỏ:</span><span class="sxs-lookup"><span data-stu-id="89b18-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="89b18-104">**Người dùng đơn**</span><span class="sxs-lookup"><span data-stu-id="89b18-104">**Single User**</span></span>
  
<span data-ttu-id="89b18-105">Thiết lập hộp thư-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="89b18-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="89b18-106">**Tổ chức**</span><span class="sxs-lookup"><span data-stu-id="89b18-106">**Organization**</span></span>
  
<span data-ttu-id="89b18-107">Get-hộp thư-ResultSize không giới hạn-lọc {RecipientTypeDetails-EQ "UserMailbox"} | Thiết lập hộp thư-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="89b18-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="89b18-108">Tìm hiểu thêm</span><span class="sxs-lookup"><span data-stu-id="89b18-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

