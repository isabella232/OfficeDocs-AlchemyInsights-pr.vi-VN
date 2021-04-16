---
title: Bật kiểm tra hộp thư
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: c04f27edc1e22e0e4269758827d5468767967be8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814214"
---
# <a name="enable-mailbox-auditing"></a>Bật kiểm tra hộp thư

Để bật kiểm tra hộp thư cho một người dùng duy nhất hoặc toàn bộ tổ chức các lệnh ghép ngắn sau đây phải được chạy từ Remote Power Shell:
  
 **Người dùng duy nhất**
  
Set-Mailbox-danh tính "Jane Dow"-AuditEnabled $true
  
 **Cấu**
  
Get-Mailbox-ResultSize không giới hạn-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Set-Mailbox-AuditEnabled $true
  
[Tìm hiểu thêm](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

