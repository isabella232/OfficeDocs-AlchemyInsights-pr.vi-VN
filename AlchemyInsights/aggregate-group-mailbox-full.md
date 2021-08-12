---
title: AggregateGroupMailbox NDR đầy đủ nhận được cho email được gửi Microsoft 365 nhóm
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
ms.openlocfilehash: 6655bbe9482400eeb3cfdf0b91bdc595e3d98fbff0f6d9244db8bb4dd958305e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951875"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox NDR đầy đủ nhận được cho email được gửi Microsoft 365 nhóm

Sử dụng lệnh EXO Shell sau đây để tạo quy Exchange truyền dẫn thư thành im lặng để thả email được gửi đến hộp thư nhóm tổng hợp:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Thay thế địa chỉ SMTP trong **-SentTo bằng địa** chỉ SMTP của hộp thư nhóm tổng hợp trong đối tượng thuê của bạn. Bạn có thể lấy địa chỉ SMTP của hộp thư nhóm tổng hợp từ NDR nhận được.



