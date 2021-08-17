---
title: Mã hóa với quy tắc truyền tải
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079472"
---
# <a name="encryption-with-transport-rules"></a>Mã hóa với quy tắc truyền tải

Trong Trung [Exchange Quản](https://go.microsoft.com/fwlink/p/?linkid=834822) trị Thư (EAC), bạn có thể sử dụng Office năng Mã hóa Thư (OME) trong quy tắc dòng thư của mình để kích hoạt mã hóa thư. Chọn tùy **chọn Áp Mã hóa Thư Office 365 quyền và bảo vệ bằng quyền** trên điều kiện Quy tắc Truyền tải.

- Để biết thêm thông tin, xem [mục Xác định quy tắc dòng Thư để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Trong Powershell, sử dụng [lệnh ghép ngắn New-TransportRule,](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) rồi đặt tham *số ApplyOME* thành $true.
