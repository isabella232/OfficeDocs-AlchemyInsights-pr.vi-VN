---
title: Người gửi không nhận được email được gửi đến Microsoft 365 nhóm
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 893b80567567590357a638370b8c8d58b87a98a51c68cfcc84629eda5ac71b44
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958319"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Người gửi không nhận được email được gửi đến Microsoft 365 nhóm

Theo mặc định, người gửi thư email đến một nhóm Microsoft 365 không nhận được bản sao của thư trong Hộp thư đến của họ, ngay cả khi người gửi là thành viên của nhóm.

Sử dụng lệnh PowerShell EXO này để cho phép người gửi nhận bản sao của từng email họ gửi đến nhóm Microsoft 365 chủ:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Để bật cài đặt cho tất cả các hộp thư cùng một lúc:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Lưu ý** Phải mất tới một giờ để thay đổi thiết đặt này có hiệu lực.