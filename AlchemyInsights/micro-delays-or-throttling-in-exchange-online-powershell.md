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
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro delays or throttling in Exchange Online PowerShell

Bạn có thể thấy cảnh báo "Áp dụng micro độ trễ" hoặc trì hoãn khi chạy tập lệnh và lệnh ghép ngắn trong Exchange Online. Dưới đây là một vài gợi ý cách giải quyết điều này:

- Vui lòng chạy chẩn đoán của chúng tôi để thư giãn các chính sách điều chỉnh PowerShell của đối tượng thuê của bạn. Giải pháp này sẽ giải quyết vấn đề trên hầu hết mọi người.
- Nếu sự cố vẫn chưa được giải quyết, hãy sử dụng mô-đun [Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)bao gồm các lệnh ghép ngắn dựa trên API REST và hoạt động tốt hơn đáng kể. Đây có thể là giải pháp tuyệt vời cho nhiều Lệnh ghép ngắn Get-lệnh ghép ngắn thường xuyên được sử dụng.
- Nếu bạn cần sử dụng lệnh ghép ngắn không được đề cập trong mô-đun v2, vui lòng xem chạy lệnh ghép ngắn [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cho số lượng lớn người dùng trong Office 365 , mục này sẽ nói về cách tránh các giới hạn điều chỉnh PowerShell trong Exchange Online.
