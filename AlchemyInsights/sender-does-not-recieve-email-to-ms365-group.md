---
title: Người gửi không nhận được email được gửi đến nhóm Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872328"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Người gửi không nhận được email được gửi đến nhóm Microsoft 365

Theo mặc định, người gửi email đến một nhóm Microsoft 365 không nhận được một bản sao của thư trong hộp thư đến của họ, ngay cả khi người gửi là thành viên của nhóm.

Sử dụng lệnh EXO PowerShell này để cho phép người gửi nhận được một bản sao của mỗi email mà họ gửi đến nhóm Microsoft 365:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Để kích hoạt cài đặt cho tất cả các hộp thư cùng một lúc:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Ghi chú** Các thay đổi đối với thiết đặt này sẽ mất đến một giờ để có hiệu lực.