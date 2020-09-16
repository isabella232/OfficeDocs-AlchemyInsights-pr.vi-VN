---
title: Đồng bộ UPN bị vô hiệu hóa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749536"
---
# <a name="upn-sync-disabled"></a>Đồng bộ UPN bị vô hiệu hóa

Nếu bạn đã bắt đầu đồng bộ với Azure AD trước ngày 30 tháng 3, 2016, hãy chạy lệnh ghép ngắn Azure AD PowerShell sau đây để bật khớp với khớp mềm UPN cho tổ chức của bạn:
  
 **Thiết lập-MsolDirSyncFeature-tính năng EnableSoftMatchOnUpn-bật $True**
  
Khớp mềm UPN được tự động bật cho các tổ chức bắt đầu đồng bộ với Azure AD vào hoặc sau ngày 30 tháng 3, 2016.
  
Để tìm hiểu thêm về việc bật tính năng khớp mềm trên UPN và các tính năng đồng bộ khác, vui lòng xem [AZURE AD Connect Sync Service](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

