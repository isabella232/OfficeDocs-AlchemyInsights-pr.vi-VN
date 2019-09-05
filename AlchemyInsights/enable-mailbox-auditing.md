---
title: Bật kiểm tra hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736275"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="88f69-102">Bật kiểm tra hộp thư</span><span class="sxs-lookup"><span data-stu-id="88f69-102">Enable mailbox auditing</span></span>

<span data-ttu-id="88f69-103">Để kích hoạt hộp kiểm tra cho người dùng hoặc một tổ chức toàn bộ các lệnh ghép ngắn sau đây phải được chạy từ xa điện vỏ:</span><span class="sxs-lookup"><span data-stu-id="88f69-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="88f69-104">**Người dùng đơn**</span><span class="sxs-lookup"><span data-stu-id="88f69-104">**Single User**</span></span>
  
<span data-ttu-id="88f69-105">Thiết lập hộp thư-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="88f69-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="88f69-106">**Tổ chức**</span><span class="sxs-lookup"><span data-stu-id="88f69-106">**Organization**</span></span>
  
<span data-ttu-id="88f69-107">Get-hộp thư-ResultSize không giới hạn-lọc {RecipientTypeDetails-EQ "UserMailbox"} | Thiết lập hộp thư-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="88f69-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="88f69-108">Tìm hiểu thêm</span><span class="sxs-lookup"><span data-stu-id="88f69-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

