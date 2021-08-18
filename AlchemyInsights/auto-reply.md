---
title: 'Để cấu hình trả lời tự động cho tất cả email được gửi Microsoft 365 nhóm:'
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331553"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>Để cấu hình trả lời tự động cho tất cả email được gửi Microsoft 365 nhóm:

**Kết nối sử dụng PowerShell của EXO bằng tài khoản người quản trị đối tượng thuê và sử dụng lệnh sau đây:**

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**Ghi** chú : Thay **đổi groupmailbox** thành tên nhóm mà bạn muốn cấu hình trả lời tự động.

