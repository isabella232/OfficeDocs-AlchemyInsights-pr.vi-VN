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
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868556"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro delays or throttling in Exchange Online PowerShell

Bạn có thể thấy cảnh báo "Áp dụng micro độ trễ" hoặc trì hoãn khi chạy tập lệnh và lệnh ghép ngắn trong Exchange Online. Dưới đây là một vài gợi ý cách giải quyết điều này:

- Vui lòng chạy chẩn đoán của chúng tôi để thư giãn các chính sách điều chỉnh PowerShell của đối tượng thuê của bạn. Giải pháp này sẽ giải quyết vấn đề trên hầu hết mọi người.
- Nếu sự cố vẫn chưa được giải quyết, hãy sử dụng mô-đun [Exchange Online v2 PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)bao gồm các lệnh ghép ngắn dựa trên API REST và hoạt động tốt hơn đáng kể. Đây có thể là giải pháp tuyệt vời cho nhiều Lệnh ghép ngắn Get-lệnh ghép ngắn thường xuyên được sử dụng.
- Nếu bạn cần sử dụng lệnh ghép ngắn không được đề cập trong mô-đun v2, vui lòng xem chạy các lệnh ghép ngắn [PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)cho số lượng lớn người dùng trong Office 365 , mục này sẽ nói về cách tránh các giới hạn điều chỉnh PowerShell trong Exchange Online.
