---
title: Các sự cố về đăng nhập vào Microsoft 365 dụng
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744668"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Sự cố đăng nhập vào Ứng dụng Microsoft 365

Lưu ý: Nếu bạn đang sử dụng phiên bản cũ hơn của Windows (ví dụ: Windows 7 SP1, [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) Windows Server 2008 R2), hãy sử dụng bản sửa lỗi dễ dàng để bật TLS 1.2 làm mặc định. Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)làm giao thức bảo mật mặc định trong WinHTTP trong Windows.

Để khắc phục sự cố đăng nhập với ứng Microsoft 365, hãy thử các tùy chọn sau trên máy bị ảnh hưởng:  

- Để biết Windows tin, [hãy Đề xuất cách giải quyết các sự cố đăng nhập phổ biến](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Đối với máy Mac, [xem mục Không thể đăng nhập vào ứng dụng Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Mẹo** Trên Windows tính, chúng tôi có thể chẩn đoán và tự động khắc phục một số sự cố Office đăng nhập thường gặp cho bạn. Tải xuống và chạy Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ **[công cụ](https://aka.ms/SaRA-OfficeSignInScenario)** tự động của chúng tôi.

**Lưu ý:** Không khuyến khích bạn vô hiệu hóa Xác thực Hiện đại (ADAL) hoặc Quản lý Tài khoản Web (WAM) để khắc phục các sự cố về đăng nhập hoặc **kích hoạt.** Nếu lỗi xảy ra trong khi kết nối với máy Microsoft 365 sử dụng [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) Office 2013, hãy đảm bảo rằng bạn bật xác thực hiện đại cho máy Office khách.

Để biết các hành động khắc phục sự cố cụ thể, hãy xem:

[Các sự cố kết nối trong đăng nhập sau khi cập nhật lên Office 2016 bản dựng 16.0.7967 trên Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Bạn không thể đăng nhập vào tài khoản tổ chức của mình, như Office 365, Azure hoặc Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Cách khắc phục sự cố ứng dụng không phải trình duyệt không thể đăng nhập vào Office 365, Azure hoặc Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Nhiều lần nhắc nhập thông tin xác thực trong Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)