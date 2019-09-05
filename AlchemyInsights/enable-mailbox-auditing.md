---
title: Bật kiểm tra hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736275"
---
# <a name="enable-mailbox-auditing"></a>Bật kiểm tra hộp thư

Để kích hoạt hộp kiểm tra cho người dùng hoặc một tổ chức toàn bộ các lệnh ghép ngắn sau đây phải được chạy từ xa điện vỏ:
  
 **Người dùng đơn**
  
Thiết lập hộp thư-Identity "Jane Dow"-AuditEnabled $true
  
 **Tổ chức**
  
Get-hộp thư-ResultSize không giới hạn-lọc {RecipientTypeDetails-EQ "UserMailbox"} | Thiết lập hộp thư-AuditEnabled $true
  
[Tìm hiểu thêm](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

