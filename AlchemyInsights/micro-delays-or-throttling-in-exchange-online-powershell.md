---
title: Vi trì hoãn hoặc điều chỉnh trong Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/30/2020
ms.locfileid: "43948025"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="1cd0f-102">Vi trì hoãn hoặc điều chỉnh trong Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="1cd0f-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="1cd0f-103">Bạn có thể thấy cảnh báo "vi trì hoãn áp dụng" hoặc chậm trễ khi bạn chạy tập lệnh và lệnh ghép ngắn trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1cd0f-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="1cd0f-104">Dưới đây là hai đề xuất liên quan đến điều này:</span><span class="sxs-lookup"><span data-stu-id="1cd0f-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="1cd0f-105">Bạn có thể muốn thử sử dụng [mô-đun Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), bao gồm các lệnh ghép ngắn dựa trên Rest API và performant đáng kể hơn.</span><span class="sxs-lookup"><span data-stu-id="1cd0f-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="1cd0f-106">Điều này có thể là một giải pháp tuyệt vời cho rất nhiều Get-lệnh ghép ngắn mà thường được sử dụng.</span><span class="sxs-lookup"><span data-stu-id="1cd0f-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="1cd0f-107">Nếu bạn cần sử dụng lệnh ghép ngắn không được bao gồm trong mô-đun v2, hãy xem [chạy lệnh ghép ngắn PowerShell cho số lượng lớn của người dùng trong Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), mà nói về làm thế nào để có được khoảng dự kiến PowerShell điều chỉnh giới hạn trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1cd0f-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
