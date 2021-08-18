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
ms.openlocfilehash: fc953813a94c9ed3226f81f776d6085e12a6cafc
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320378"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Đặt ClientAccessServerEnabled thành True

Nếu bạn không thể mở thư email đã mã hóa và thay vào đó hãy xem phần đính kèm **rpmsg,** hãy thực hiện các bước sau đây:

1. Kết nối đổi Exchange Online với PowerShell.

    **Lưu** ý: Để kết nối với PowerShell Exchange Online, bạn phải đăng nhập bằng người quản trị toàn cầu hoặc tài khoản người quản Exchange toàn cầu.

   a. Mở Windows PowerShell tệp, rồi chạy lệnh sau đây:`$UserCredential = Get-Credential`
   b. Trong hộp thoại **Windows PowerShell Yêu cầu Thông tin xác thực,** nhập tài khoản cơ quan hoặc trường học và mật khẩu của bạn, c. Bấm **OK**. 

2. Chạy lệnh sau đây để tạo phiên mới:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Chạy lệnh sau:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Lệnh `Get-IRMConfiguration` Chạy.

4. Kiểm tra **cài đặt ClientAccessServerEnabled.** 

    a. Nếu **cài đặt ClientAccessServerEnabled** được đặt thành **False**, hãy chạy lệnh ghép ngắn sau đây: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

**Mẹo**: Luôn đóng phiên powershell của bạn với lệnh sau đây: `Remove-PSSession $Session`

Để biết thêm thông tin, [hãy Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

