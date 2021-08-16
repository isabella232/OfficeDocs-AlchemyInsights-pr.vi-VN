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
ms.openlocfilehash: 6646ca4792ac4d9fb8bfb7433d53ecf4aeba8da0aca797225c16c02b28499889
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013266"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a>Các sự cố khi cài đặt Bộ bảo vệ Microsoft trên máy Mac hoặc Linux

**Máy Mac**

- Đảm bảo đáp ứng các yêu cầu hệ thống trước khi cài đặt ATP của Bộ bảo vệ Microsoft cho máy Mac. Để biết thêm thông tin, xem [mục Cách cài đặt ATP của Bộ bảo vệ Microsoft dành cho máy Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).  
- Xem lại thông tin trong tệp: "/Thư viện/Nhật ký/Microsoft/mdatp/install.log".

**Linux**

- Hãy đảm bảo đáp ứng các yêu cầu hệ thống trước khi cài đặt ATP của Bộ bảo vệ Microsoft cho Linux. Để biết thêm thông tin, [xem mục Cách cài đặt MDATP cho Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements). 
- Để xác minh rằng dịch vụ MDATP đang chạy, hãy xem cài [đặt không thành công.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)  
    Để khắc phục sự cố và giải quyết các vấn đề nếu dịch vụ không chạy, hãy xem Các bước để khắc phục sự cố nếu [dịch vụ mdatp không chạy](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).
- Để biết các bước kiểm tra cấu hình máy khách, giúp kiểm tra tình trạng sản phẩm và chạy kiểm tra phát hiện trên tệp văn bản EICAR, hãy xem [Cấu hình máy khách](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).  

    **Lưu ý** Để biết danh sách các hệ thống tệp được hỗ trợ cho hoạt động truy nhập vào, hãy xem [mục ATP của Bộ bảo vệ Microsoft cho Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)