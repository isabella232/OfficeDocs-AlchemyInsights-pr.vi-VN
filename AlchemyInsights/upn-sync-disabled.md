---
title: Đã tắt đồng bộ UPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038134"
---
# <a name="upn-sync-disabled"></a>Đã tắt đồng bộ UPN

Nếu bạn đã bắt đầu đồng bộ với Azure AD trước 30/03/2016, hãy chạy lệnh ghép ngắn Azure AD PowerShell sau đây để chỉ bật kết quả khớp mềm UPN cho tổ chức của bạn:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
Kết quả khớp mềm UPN được bật tự động cho các tổ chức bắt đầu đồng bộ hóa với Azure AD vào hoặc sau ngày 30 tháng 3 năm 2016.
  
Để tìm hiểu thêm về cách bật kết quả khớp mềm trên UPN và các tính năng đồng bộ khác, vui lòng xem [mục Azure AD Kết nối năng dịch vụ đồng bộ.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

