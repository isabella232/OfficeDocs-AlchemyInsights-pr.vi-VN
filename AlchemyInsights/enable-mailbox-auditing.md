---
title: Bật kiểm tra hộp thư
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
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 404ef9ecd824541f98471bb8797f5f6e025012b7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806313"
---
# <a name="enable-mailbox-auditing"></a>Bật kiểm tra hộp thư

Để bật kiểm tra hộp thư cho một người dùng duy nhất hoặc toàn bộ tổ chức các lệnh ghép ngắn sau đây phải được chạy từ Remote Power Shell:
  
 **Người dùng duy nhất**
  
Set-Mailbox-Identity "Jane Dow"-kiểm tra $true
  
 **Cấu**
  
Get-Mailbox-ResultSize không giới hạn-Filter {RecipientTypeDetails-EQ "UserMailbox"} | Đặt-hộp thư-kiểm tra $true
  
[Tìm hiểu thêm](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

