---
title: Sự cố với SharePoint trên Windows 7 máy
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125780"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Sự cố với SharePoint trên Windows 7 máy

Nếu bạn nhận được lỗi trên máy Windows 7 trong khi làm việc trên SharePoint hoặc OneDrive, chúng có thể liên quan đến việc TLS 1.0/1 bị bỏ dùng. Để biết thêm thông tin, hãy xem:

- [Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows khách 7 SP1/Windows 8 khách phải được bật TLS1.2. Để biết thêm thông tin, [hãy xem mục Lỗi xác thực xảy ra khi máy khách không có hỗ trợ TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Cài đặt KB3140245 và tạo giá trị sổ đăng ký. Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) làm giao thức bảo mật mặc định trong WinHTTP trong Windows

- Windows khách 7 SP1/Windows 8 phải đảm bảo cài đặt bộ mã VLS mới nhất. Để biết thêm thông tin, [hãy xem mục Tư vấn Bảo mật Microsoft 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058) 


