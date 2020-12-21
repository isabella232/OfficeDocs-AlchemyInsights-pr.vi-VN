---
title: AggregateGroupMailbox đã nhận được NDR đầy đủ cho email được gửi đến nhóm Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722074"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="a7a95-102">AggregateGroupMailbox đã nhận được NDR đầy đủ cho email được gửi đến nhóm Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a7a95-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="a7a95-103">Sử dụng lệnh EXO Shell sau đây để tạo quy tắc truyền dẫn Exchange để âm thanh thả email được gửi đến hộp thư nhóm tổng hợp:</span><span class="sxs-lookup"><span data-stu-id="a7a95-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="a7a95-104">Thay thế địa chỉ SMTP trong **-sentto** với địa chỉ SMTP của hộp thư nhóm tổng hợp trong đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="a7a95-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="a7a95-105">Bạn có thể nhận được địa chỉ SMTP của hộp thư nhóm tổng hợp từ NDR đã nhận được.</span><span class="sxs-lookup"><span data-stu-id="a7a95-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



