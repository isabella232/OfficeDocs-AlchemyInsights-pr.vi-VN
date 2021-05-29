---
title: Micro delays or throttling in Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702148"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="b72f1-102">Micro delays or throttling in Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="b72f1-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="b72f1-103">Bạn có thể thấy cảnh báo "Áp dụng micro độ trễ" hoặc trì hoãn khi chạy tập lệnh và lệnh ghép ngắn trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b72f1-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="b72f1-104">Dưới đây là một vài gợi ý cách giải quyết điều này:</span><span class="sxs-lookup"><span data-stu-id="b72f1-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="b72f1-105">Vui lòng chạy chẩn đoán của chúng tôi để thư giãn các chính sách điều chỉnh PowerShell của đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="b72f1-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="b72f1-106">Giải pháp này sẽ giải quyết vấn đề trên hầu hết mọi người.</span><span class="sxs-lookup"><span data-stu-id="b72f1-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="b72f1-107">Nếu sự cố vẫn chưa được giải quyết, hãy sử dụng mô-đun [Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)bao gồm các lệnh ghép ngắn dựa trên API REST và hoạt động tốt hơn đáng kể.</span><span class="sxs-lookup"><span data-stu-id="b72f1-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="b72f1-108">Đây có thể là giải pháp tuyệt vời cho nhiều Lệnh ghép ngắn Get-lệnh ghép ngắn thường xuyên được sử dụng.</span><span class="sxs-lookup"><span data-stu-id="b72f1-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="b72f1-109">Nếu bạn cần sử dụng lệnh ghép ngắn không được đề cập trong mô-đun v2, vui lòng xem chạy lệnh ghép ngắn [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cho số lượng lớn người dùng trong Office 365 , mục này sẽ nói về cách tránh các giới hạn điều chỉnh PowerShell trong Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b72f1-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
