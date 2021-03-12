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
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Các sự cố khi cài đặt Microsoft Defender trên máy Mac hoặc Linux

**Ana**

- Đảm bảo rằng các yêu cầu hệ thống được đáp ứng trước khi cài đặt Microsoft Defender ATP cho Mac. Để biết thêm thông tin, hãy xem [cách cài đặt Microsoft Defender ATP cho Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Xem lại thông tin trong tệp: "/Library/Logs/Microsoft/mdatp/install.log".

**Windows**

- Đảm bảo rằng các yêu cầu hệ thống được đáp ứng trước khi cài đặt Microsoft Defender ATP cho Linux. Để biết thêm thông tin, hãy xem [cách cài đặt Microsoft Defender ATP cho Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Để xác minh rằng dịch vụ MDATP đang chạy, hãy xem [cài đặt không](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)thành công.  
    Để khắc phục sự cố và giải quyết vấn đề nếu dịch vụ không chạy, hãy xem các [bước khắc phục sự cố nếu không chạy dịch vụ mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Để biết các bước để kiểm tra cấu hình máy khách, điều này sẽ xác minh tình trạng của sản phẩm và để chạy thử nghiệm phát hiện trên tệp văn bản EICAR, hãy xem [cấu hình máy khách](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Ghi chú** Để biết danh sách các hệ thống tệp được hỗ trợ cho hoạt động trên Access, hãy xem [Microsoft Defender ATP cho Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).