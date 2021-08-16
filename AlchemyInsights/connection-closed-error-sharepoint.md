---
title: Kết nối cơ sở đã bị đóng lỗi trong SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044434"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Lỗi "Đã đóng kết nối cơ sở" trong SharePoint

Nếu bạn đang nhận được lỗi "Đã đóng kết nối cơ sở" trong SharePoint điều này có thể liên quan đến việc bỏ dùng TLS 1.0/1.1. Để biết thêm thông tin, hãy xem các bài viết sau:

- [Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Lỗi xác thực xảy ra nếu máy khách không có hỗ trợ TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Cập nhật để bật TLS 1.1 và TLS 1.2 làm giao thức bảo mật mặc định trong WinHTTP trong Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Nếu người dùng đang sử Windows 7, hãy đảm bảo họ đánh dấu chọn [TLS Cipher Suites trong Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)