---
title: Cấu hình loại trừ cho bộ quét ATP của Microsoft Defender
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714357"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="ac2ab-102">Cấu hình loại trừ cho bộ quét ATP của Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="ac2ab-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="ac2ab-103">Nói chung, bạn có thể loại trừ các phần mở rộng tệp nhất định và các vị trí thư mục từ quét bộ ATP của Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="ac2ab-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="ac2ab-104">Bạn cũng có thể cấu hình loại trừ cho các tệp được mở bởi các quy trình nhất định.</span><span class="sxs-lookup"><span data-stu-id="ac2ab-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="ac2ab-105">Để biết thêm thông tin, hãy xem, [cấu hình và xác thực các loại trừ dựa trên phần mở rộng tệp và vị trí thư mục](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) và [đặt cấu hình các loại trừ cho các tệp được mở theo quy trình](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="ac2ab-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="ac2ab-106">Để cấu hình loại trừ cho  **Windows server 2016 và 2019**, hãy xem [cấu hình các loại trừ chống virus của Microsoft Defender trên Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="ac2ab-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ac2ab-107">**Ana**</span><span class="sxs-lookup"><span data-stu-id="ac2ab-107">**Mac**</span></span>

<span data-ttu-id="ac2ab-108">Để biết chi tiết về các kiểu loại trừ được hỗ trợ và cấu hình một danh sách các loại trừ cho Mac, hãy xem các [kiểu loại trừ được hỗ trợ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) và [cách cấu hình danh sách loại trừ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="ac2ab-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="ac2ab-109">**Ghi chú** Bạn cũng có thể xác thực các danh sách loại trừ bằng cách dùng tệp kiểm tra EICAR.</span><span class="sxs-lookup"><span data-stu-id="ac2ab-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ac2ab-110">Để biết thêm thông tin, hãy xem [xác thực danh sách loại trừ có tệp kiểm tra EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ac2ab-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="ac2ab-111">**Windows**</span><span class="sxs-lookup"><span data-stu-id="ac2ab-111">**Linux**</span></span>

<span data-ttu-id="ac2ab-112">Để biết chi tiết về các kiểu loại trừ được hỗ trợ và cấu hình một danh sách các loại trừ cho Linux, hãy xem các kiểu loại trừ và cấu hình [được hỗ trợ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) và xác thực các loại [trừ cho Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="ac2ab-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="ac2ab-113">**Ghi chú** Bạn cũng có thể xác thực các danh sách loại trừ bằng cách dùng tệp kiểm tra EICAR.</span><span class="sxs-lookup"><span data-stu-id="ac2ab-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ac2ab-114">Để biết thêm thông tin, hãy xem [xác thực danh sách loại trừ có tệp kiểm tra EICAR](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ac2ab-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 