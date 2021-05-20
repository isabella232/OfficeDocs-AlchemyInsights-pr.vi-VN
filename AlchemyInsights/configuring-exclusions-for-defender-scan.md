---
title: Đặt cấu hình loại trừ để ATP của Bộ bảo vệ Microsoft quét
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543707"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="ae043-102">Đặt cấu hình loại trừ để ATP của Bộ bảo vệ Microsoft quét</span><span class="sxs-lookup"><span data-stu-id="ae043-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="ae043-103">Thông thường, bạn có thể loại trừ một số phần mở rộng tệp và vị trí thư mục ATP của Bộ bảo vệ Microsoft khi quét.</span><span class="sxs-lookup"><span data-stu-id="ae043-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="ae043-104">Bạn cũng có thể cấu hình loại trừ cho tệp được mở bằng quy trình nhất định.</span><span class="sxs-lookup"><span data-stu-id="ae043-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="ae043-105">Để biết thêm thông tin, hãy xem [Cấu](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) hình và xác thực loại trừ dựa trên vị trí phần mở rộng tệp và thư mục và Đặt cấu hình loại trừ cho các tệp [được mở bằng quy trình.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="ae043-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="ae043-106">Để đặt cấu hình loại trừ **cho Windows Server 2016 và 2019,** hãy xem đặt cấu [hình loại Tính năng Chống Virut của Bộ bảo vệ Microsoft](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)loại trừ Windows Server .</span><span class="sxs-lookup"><span data-stu-id="ae043-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="ae043-107">**Máy Mac**</span><span class="sxs-lookup"><span data-stu-id="ae043-107">**Mac**</span></span>

<span data-ttu-id="ae043-108">Để biết chi tiết về các loại loại trừ được hỗ trợ [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) và cấu hình danh sách loại trừ cho máy Mac, hãy xem Các loại loại trừ được hỗ trợ và Cách cấu hình danh sách loại [trừ.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="ae043-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="ae043-109">**Lưu ý** Bạn cũng có thể xác thực danh sách loại trừ bằng cách dùng tệp kiểm tra EICAR.</span><span class="sxs-lookup"><span data-stu-id="ae043-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ae043-110">Để biết thêm thông tin, [hãy xem Mục Xác thực danh sách loại trừ bằng tệp kiểm tra EICAR](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ae043-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="ae043-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="ae043-111">**Linux**</span></span>

<span data-ttu-id="ae043-112">Để biết chi tiết về các loại loại trừ được hỗ trợ [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) và cấu hình danh sách loại trừ cho Linux, hãy xem Các loại loại trừ được hỗ trợ và Đặt cấu hình và xác thực loại trừ [cho ATP của Bộ bảo vệ Microsoft cho Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="ae043-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="ae043-113">**Lưu ý** Bạn cũng có thể xác thực danh sách loại trừ bằng cách dùng tệp kiểm tra EICAR.</span><span class="sxs-lookup"><span data-stu-id="ae043-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="ae043-114">Để biết thêm thông tin, [hãy xem Mục Xác thực danh sách loại trừ bằng tệp kiểm tra EICAR](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="ae043-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 