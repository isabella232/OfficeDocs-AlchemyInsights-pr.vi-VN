---
title: Các sự cố khi cài đặt Microsoft Defender trên máy Mac hoặc Linux
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
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "50714321"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="dc8cb-102">Các sự cố khi cài đặt Microsoft Defender trên máy Mac hoặc Linux</span><span class="sxs-lookup"><span data-stu-id="dc8cb-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="dc8cb-103">**Ana**</span><span class="sxs-lookup"><span data-stu-id="dc8cb-103">**Mac**</span></span>

- <span data-ttu-id="dc8cb-104">Đảm bảo rằng các yêu cầu hệ thống được đáp ứng trước khi cài đặt Microsoft Defender ATP cho Mac.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="dc8cb-105">Để biết thêm thông tin, hãy xem [cách cài đặt Microsoft Defender ATP cho Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="dc8cb-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="dc8cb-106">Xem lại thông tin trong tệp: "/Library/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="dc8cb-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="dc8cb-107">**Windows**</span><span class="sxs-lookup"><span data-stu-id="dc8cb-107">**Linux**</span></span>

- <span data-ttu-id="dc8cb-108">Đảm bảo rằng các yêu cầu hệ thống được đáp ứng trước khi cài đặt Microsoft Defender ATP cho Linux.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="dc8cb-109">Để biết thêm thông tin, hãy xem [cách cài đặt Microsoft Defender ATP cho Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="dc8cb-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="dc8cb-110">Để xác minh rằng dịch vụ MDATP đang chạy, hãy xem [cài đặt không](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)thành công.</span><span class="sxs-lookup"><span data-stu-id="dc8cb-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="dc8cb-111">Để khắc phục sự cố và giải quyết vấn đề nếu dịch vụ không chạy, hãy xem các [bước khắc phục sự cố nếu không chạy dịch vụ mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="dc8cb-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="dc8cb-112">Để biết các bước để kiểm tra cấu hình máy khách, điều này sẽ xác minh tình trạng của sản phẩm và để chạy thử nghiệm phát hiện trên tệp văn bản EICAR, hãy xem [cấu hình máy khách](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="dc8cb-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="dc8cb-113">**Ghi chú** Để biết danh sách các hệ thống tệp được hỗ trợ cho hoạt động trên Access, hãy xem [Microsoft Defender ATP cho Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="dc8cb-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>