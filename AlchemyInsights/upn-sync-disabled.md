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
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532353"
---
# <a name="upn-sync-disabled"></a>Đồng bộ UPN bị vô hiệu hoá

Nếu bạn bắt đầu đồng bộ hoá với các quảng cáo Azure trước ngày 30 tháng 3 năm 2016, chạy lệnh ghép ngắn PowerShell Azure quảng cáo sau đây để sử UPN mềm mại phù hợp cho tổ chức của bạn chỉ:
  
 **Thiết lập MsolDirSyncFeature-có EnableSoftMatchOnUpn-sử $True**
  
UPN mềm phù hợp sẽ được bật cho các tổ chức bắt đầu đồng bộ hoá quảng cáo Azure vào hoặc sau ngày 30 tháng 3 năm 2016.
  
Để tìm hiểu thêm về bật mềm trận trên UPN và các tính năng đồng bộ hóa, hãy xem [tính năng dịch vụ Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

