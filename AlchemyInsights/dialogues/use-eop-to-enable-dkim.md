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
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527222"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="cfc1d-102">Sử dụng Exchange Online PowerShell để bật hàm IKIM cho một tên miền cụ thể</span><span class="sxs-lookup"><span data-stu-id="cfc1d-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="cfc1d-103">Nếu bạn không thể tạo bản ghi DNS của hàm trong Trung tâm quản trị, hãy thử sử dụng Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cfc1d-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="cfc1d-104">Để tạo bản ghi DNS của bkim bằng Exchange Online PowerShell, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="cfc1d-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="cfc1d-105">Mở Windows PowerShell với tư thế là người quản trị và chạy các lệnh sau đây trong trình tự được mô tả:</span><span class="sxs-lookup"><span data-stu-id="cfc1d-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="cfc1d-106">một.</span><span class="sxs-lookup"><span data-stu-id="cfc1d-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="cfc1d-107">b.</span><span class="sxs-lookup"><span data-stu-id="cfc1d-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="cfc1d-108">c's.</span><span class="sxs-lookup"><span data-stu-id="cfc1d-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="cfc1d-109">Nếu bạn gặp sự cố khi kết nối với Exchange Online PowerShell, hãy xem [kết nối với Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="cfc1d-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="cfc1d-110">Sau khi bạn đã kết nối với Exchange Online PowerShell, hãy chạy lệnh sau đây:</span><span class="sxs-lookup"><span data-stu-id="cfc1d-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="cfc1d-111">Sau khi lệnh trên đã được thực hiện thành công, hãy chạy lệnh sau đây để chấm dứt phiên Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cfc1d-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



