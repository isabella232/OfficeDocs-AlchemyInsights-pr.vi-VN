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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Vi trì hoãn hoặc điều chỉnh trong Exchange Online PowerShell

Bạn có thể thấy cảnh báo "vi trì hoãn áp dụng" hoặc chậm trễ khi bạn chạy tập lệnh và lệnh ghép ngắn trong Exchange Online. Dưới đây là hai đề xuất liên quan đến điều này:

- Bạn có thể muốn thử sử dụng [mô-đun Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), bao gồm các lệnh ghép ngắn dựa trên Rest API và performant đáng kể hơn. Điều này có thể là một giải pháp tuyệt vời cho rất nhiều Get-lệnh ghép ngắn mà thường được sử dụng.
- Nếu bạn cần sử dụng lệnh ghép ngắn không được bao gồm trong mô-đun v2, hãy xem [chạy lệnh ghép ngắn PowerShell cho số lượng lớn của người dùng trong Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), mà nói về làm thế nào để có được khoảng dự kiến PowerShell điều chỉnh giới hạn trong Exchange Online.
