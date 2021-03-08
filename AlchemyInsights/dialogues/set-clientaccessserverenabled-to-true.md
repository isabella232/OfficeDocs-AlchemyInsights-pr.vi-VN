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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527415"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Đặt ClientAccessServerEnabled thành True

Nếu bạn không thể mở thư email đã mã hóa và thay vào đó, hãy xem phần đính kèm **rpmsg** , thực hiện các bước sau đây:

1. Kết nối với Exchange Online PowerShell.

> [!NOTE]
> Để kết nối với Exchange Online PowerShell, bạn phải đăng nhập bằng tài khoản người quản trị toàn cầu hoặc tài khoản người quản trị Exchange.

   một. Mở Windows PowerShell, rồi chạy lệnh sau đây: `$UserCredential = Get-Credential`
b. Trong hộp thoại yêu cầu chứng danh của **Windows PowerShell** , hãy nhập tài khoản và mật khẩu cơ quan hoặc trường học của bạn, c. Bấm **OK**. 

2. Chạy lệnh sau đây để tạo một phiên mới:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    một. Chạy lệnh sau:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Lệnh chạy.

4. Kiểm tra cài đặt **Clientaccessserverenabled** . 

    một. Nếu thiết đặt **Clientaccessserverenabled** được đặt là **false**, hãy chạy lệnh ghép ngắn sau đây: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Luôn đóng phiên PowerShell với lệnh sau đây: `Remove-PSSession $Session`

Để biết thêm thông tin, hãy xem [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

