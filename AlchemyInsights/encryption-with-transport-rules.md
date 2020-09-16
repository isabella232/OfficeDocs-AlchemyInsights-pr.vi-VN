---
title: Mã hóa với quy tắc truyền dẫn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784365"
---
# <a name="encryption-with-transport-rules"></a>Mã hóa với quy tắc truyền dẫn

Trong [Trung tâm quản trị Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), bạn có thể sử dụng các chức năng mã hóa tin nhắn Office (OME) trong các quy tắc dòng thư để kích hoạt mã hóa thư. Chọn tùy chọn **áp dụng mã hóa thư Office 365 và bảo vệ quyền** trên điều kiện quy tắc truyền dẫn.

- Để biết thêm thông tin, hãy xem mục [xác định quy tắc dòng thư để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Trong PowerShell, sử dụng lệnh ghép ngắn [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) và đặt tham số *applyome* sang $True.
