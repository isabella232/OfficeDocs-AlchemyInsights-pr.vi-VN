---
title: Đồng bộ UPN bị vô hiệu hoá
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921730"
---
# <a name="upn-sync-disabled"></a>Đồng bộ UPN bị vô hiệu hoá

Nếu bạn bắt đầu đồng bộ hoá với các quảng cáo Azure trước ngày 30 tháng 3 năm 2016, chạy lệnh ghép ngắn PowerShell Azure quảng cáo sau đây để sử UPN mềm mại phù hợp cho tổ chức của bạn chỉ:
  
 **Thiết lập MsolDirSyncFeature-có EnableSoftMatchOnUpn-sử $True**
  
UPN mềm phù hợp sẽ được bật cho các tổ chức bắt đầu đồng bộ hoá quảng cáo Azure vào hoặc sau ngày 30 tháng 3 năm 2016.
  
Để tìm hiểu thêm về bật mềm trận trên UPN và các tính năng đồng bộ hóa, hãy xem [tính năng dịch vụ Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

