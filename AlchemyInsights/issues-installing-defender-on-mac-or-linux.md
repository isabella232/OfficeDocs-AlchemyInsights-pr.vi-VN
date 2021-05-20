---
title: Các sự cố khi cài đặt Bộ bảo vệ Microsoft trên máy Mac hoặc Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539702"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="71ff7-102">Các sự cố khi cài đặt Bộ bảo vệ Microsoft trên máy Mac hoặc Linux</span><span class="sxs-lookup"><span data-stu-id="71ff7-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="71ff7-103">**Máy Mac**</span><span class="sxs-lookup"><span data-stu-id="71ff7-103">**Mac**</span></span>

- <span data-ttu-id="71ff7-104">Đảm bảo đáp ứng các yêu cầu hệ thống trước khi cài ATP của Bộ bảo vệ Microsoft for Mac.</span><span class="sxs-lookup"><span data-stu-id="71ff7-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="71ff7-105">Để biết thêm thông tin, [hãy xem Cách cài đặt ATP của Bộ bảo vệ Microsoft for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="71ff7-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="71ff7-106">Xem lại thông tin trong tệp: "/Thư viện/Nhật ký/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="71ff7-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="71ff7-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="71ff7-107">**Linux**</span></span>

- <span data-ttu-id="71ff7-108">Đảm bảo đáp ứng yêu cầu hệ thống trước khi cài ATP của Bộ bảo vệ Microsoft cho Linux.</span><span class="sxs-lookup"><span data-stu-id="71ff7-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="71ff7-109">Để biết thêm thông tin, [xem mục Cách cài đặt MDATP cho Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="71ff7-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="71ff7-110">Để xác minh rằng dịch vụ MDATP đang chạy, hãy xem cài [đặt không thành công.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="71ff7-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="71ff7-111">Để khắc phục sự cố và giải quyết các vấn đề nếu dịch vụ không chạy, hãy xem Các bước để khắc phục sự cố nếu [dịch vụ mdatp không chạy](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="71ff7-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="71ff7-112">Để biết các bước kiểm tra cấu hình máy khách, giúp kiểm tra tình trạng sản phẩm và chạy kiểm tra phát hiện trên tệp văn bản EICAR, hãy xem [Cấu hình máy khách](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="71ff7-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="71ff7-113">**Lưu ý** Để biết danh sách các hệ thống tệp được hỗ trợ cho hoạt động truy nhập vào, [hãy xem ATP của Bộ bảo vệ Microsoft cho Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="71ff7-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>