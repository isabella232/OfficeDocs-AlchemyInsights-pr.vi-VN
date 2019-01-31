---
title: Đồng bộ UPN bị vô hiệu hoá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 027782bb2a6b892df6201f3c3bf55151ef7b9db7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657993"
---
# <a name="upn-sync-disabled"></a>Đồng bộ UPN bị vô hiệu hoá

Nếu bạn bắt đầu đồng bộ hoá với các quảng cáo Azure trước ngày 30 tháng 3 năm 2016, chạy lệnh ghép ngắn PowerShell Azure quảng cáo sau đây để sử UPN mềm mại phù hợp cho tổ chức của bạn chỉ:
  
 **Thiết lập MsolDirSyncFeature-có EnableSoftMatchOnUpn-sử $True**
  
UPN mềm phù hợp sẽ được bật cho các tổ chức bắt đầu đồng bộ hoá quảng cáo Azure vào hoặc sau ngày 30 tháng 3 năm 2016.
  
Để tìm hiểu thêm về bật mềm trận trên UPN và các tính năng đồng bộ hóa, hãy xem [tính năng dịch vụ Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

