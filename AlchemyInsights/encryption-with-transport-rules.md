---
title: Mã hóa với quy tắc truyền tải
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915283"
---
# <a name="encryption-with-transport-rules"></a>Mã hóa với quy tắc truyền tải

Trong [Trung tâm quản trị Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), bạn có thể sử dụng chức năng mã hóa thư Office (OME) trong quy tắc luồng thư để kích hoạt mã hóa thư. Chọn tuỳ chọn **áp dụng Office 365 thông báo mã hóa và bảo vệ quyền** trên điều kiện quy tắc truyền tải.

- Để biết thêm thông tin, xem [xác định quy tắc luồng thư để mã hóa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Trong PowerShell, sử dụng lệnh ghép ngắn [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) và đặt tham số *applyome* $True.
