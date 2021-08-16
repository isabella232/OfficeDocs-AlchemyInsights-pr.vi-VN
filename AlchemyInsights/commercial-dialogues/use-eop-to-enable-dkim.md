---
title: Sử Exchange Online PowerShell để kích hoạt DKIM cho một miền cụ thể
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070346"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Sử Exchange Online PowerShell để kích hoạt DKIM cho một miền cụ thể

Nếu bạn không thể tạo các bản ghi DNS DKIM trong trung tâm quản trị, hãy thử sử dụng Exchange Online PowerShell. 

Để tạo bản ghi DNS DKIM bằng cách Exchange Online PowerShell, hãy thực hiện các bước sau đây:

1. Mở Windows PowerShell với tư cách người quản trị và chạy các lệnh sau theo trình tự được mô tả:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Nếu bạn gặp sự cố khi kết nối Exchange Online PowerShell, [hãy xem Kết nối kết Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Sau khi bạn đã kết nối với Exchange Online PowerShell, hãy chạy lệnh sau đây:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Sau khi lệnh ở trên đã được thực thi thành công, hãy chạy lệnh sau đây để chấm dứt Exchange Online phiên PowerShell:

    `Remove-PSSession $Session` 



