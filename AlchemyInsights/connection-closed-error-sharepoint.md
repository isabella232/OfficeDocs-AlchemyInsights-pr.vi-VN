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
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233448"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Lỗi "Đã đóng kết nối cơ sở" trong SharePoint

Nếu bạn đang nhận được lỗi "Đã đóng kết nối cơ sở" trong SharePoint điều này có thể liên quan đến việc bỏ dùng TLS 1.0/1.1. Để biết thêm thông tin, hãy xem các bài viết sau:

- [Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Lỗi xác thực xảy ra nếu máy khách không có hỗ trợ TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Nếu người dùng đang sử Windows 7, hãy đảm bảo họ đánh dấu chọn [TLS Cipher Suites trong Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)