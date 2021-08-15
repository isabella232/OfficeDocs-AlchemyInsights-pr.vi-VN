---
title: Đặt ClientAccessServerEnabled thành True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994887"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Đặt ClientAccessServerEnabled thành True

Nếu bạn không thể mở thư email đã  mã hóa và thay vào đó, hãy thực hiện các bước sau đây:

1. Kết nối để Exchange Online PowerShell.

> [!NOTE]
> Để kết nối với Exchange Online PowerShell, bạn phải đăng nhập bằng người quản trị toàn cầu hoặc tài khoản Exchange trị viên.

   a. Mở Windows PowerShell, rồi chạy lệnh sau đây:`$UserCredential = Get-Credential`
b. Trong hộp thoại **Windows PowerShell Yêu cầu Thông tin xác thực,** nhập tài khoản cơ quan hoặc trường học và mật khẩu của bạn, c. Bấm **OK**. 

2. Chạy lệnh sau đây để tạo phiên mới:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Chạy lệnh sau:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Lệnh `Get-IRMConfiguration` Chạy.

4. Kiểm tra **cài đặt ClientAccessServerEnabled.** 

    a. Nếu **cài đặt ClientAccessServerEnabled** được đặt thành **False**, hãy chạy lệnh ghép ngắn sau: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Luôn đóng phiên powershell của bạn với lệnh sau đây: `Remove-PSSession $Session`

Để biết thêm thông tin, [hãy Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

