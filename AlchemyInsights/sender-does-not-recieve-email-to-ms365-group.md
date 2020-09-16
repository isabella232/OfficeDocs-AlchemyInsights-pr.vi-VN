---
title: Người gửi không nhận được email được gửi đến nhóm Microsoft 365
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
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751337"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="c79bb-102">Người gửi không nhận được email được gửi đến nhóm Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c79bb-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="c79bb-103">Theo mặc định, người gửi email đến một nhóm Microsoft 365 không nhận được một bản sao của thư trong hộp thư đến của họ, ngay cả khi người gửi là thành viên của nhóm.</span><span class="sxs-lookup"><span data-stu-id="c79bb-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="c79bb-104">Sử dụng lệnh EXO PowerShell này để cho phép người gửi nhận được một bản sao của mỗi email mà họ gửi đến nhóm Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="c79bb-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="c79bb-105">Để kích hoạt cài đặt cho tất cả các hộp thư cùng một lúc:</span><span class="sxs-lookup"><span data-stu-id="c79bb-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="c79bb-106">**Ghi chú** Các thay đổi đối với thiết đặt này sẽ mất đến một giờ để có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="c79bb-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>