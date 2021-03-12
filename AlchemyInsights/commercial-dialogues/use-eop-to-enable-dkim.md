---
title: Sử dụng Exchange Online PowerShell để bật hàm IKIM cho một tên miền cụ thể
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749736"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Sử dụng Exchange Online PowerShell để bật hàm IKIM cho một tên miền cụ thể

Nếu bạn không thể tạo bản ghi DNS của hàm trong Trung tâm quản trị, hãy thử sử dụng Exchange Online PowerShell. 

Để tạo bản ghi DNS của bkim bằng Exchange Online PowerShell, hãy thực hiện các bước sau đây:

1. Mở Windows PowerShell với tư thế là người quản trị và chạy các lệnh sau đây trong trình tự được mô tả:

    một. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c's. `Import-PSSession $Session -DisableNameChecking`
    
Nếu bạn gặp sự cố khi kết nối với Exchange Online PowerShell, hãy xem [kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Sau khi bạn đã kết nối với Exchange Online PowerShell, hãy chạy lệnh sau đây:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Sau khi lệnh trên đã được thực hiện thành công, hãy chạy lệnh sau đây để chấm dứt phiên Exchange Online PowerShell:

    `Remove-PSSession $Session` 



