---
title: AggregateGroupMailbox NDR đầy đủ đã nhận được cho email được gửi Microsoft 365 nhóm
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
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315932"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox NDR đầy đủ đã nhận được cho email được gửi Microsoft 365 nhóm

Sử dụng lệnh EXO Shell sau đây để tạo quy tắc truyền Exchange thư thành thầm thả email được gửi đến hộp thư nhóm tổng hợp:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Ghi chú**: Thay thế địa chỉ SMTP trong **-SentTo bằng địa** chỉ SMTP của hộp thư nhóm tổng hợp trong đối tượng thuê của bạn. Bạn có thể lấy địa chỉ SMTP của hộp thư nhóm tổng hợp từ NDR nhận được.



