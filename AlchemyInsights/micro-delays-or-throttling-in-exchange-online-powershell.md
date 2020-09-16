---
title: Vi độ chậm trễ hoặc điều chỉnh trong Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743936"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="48ad0-102">Vi độ chậm trễ hoặc điều chỉnh trong Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="48ad0-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="48ad0-103">Bạn có thể thấy "Micro Delay đã áp dụng" cảnh báo hoặc sự chậm trễ khi bạn chạy các script và lệnh ghép ngắn trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="48ad0-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="48ad0-104">Dưới đây là hai đề xuất liên quan đến điều này:</span><span class="sxs-lookup"><span data-stu-id="48ad0-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="48ad0-105">Bạn có thể muốn thử sử dụng [mô-đun Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), trong đó bao gồm các lệnh ghép ngắn dựa trên API còn lại và được xem là một cách khác đáng kể.</span><span class="sxs-lookup"><span data-stu-id="48ad0-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="48ad0-106">Điều này có thể là một giải pháp tuyệt vời cho nhiều lệnh ghép ngắn được sử dụng thường xuyên.</span><span class="sxs-lookup"><span data-stu-id="48ad0-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="48ad0-107">Nếu bạn cần sử dụng các lệnh ghép ngắn không được bảo vệ trong mô-đun v2, vui lòng xem mục [chạy lệnh ghép ngắn PowerShell với số lượng lớn người dùng trong Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), mà nói về cách thức để có được khoảng giới hạn điều chỉnh của PowerShell dự kiến trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="48ad0-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
