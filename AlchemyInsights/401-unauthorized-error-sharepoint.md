---
title: 401 Lỗi trái phép trong SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233535"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Lỗi trái phép trong SharePoint

Nếu bạn nhận được lỗi "(401) Trái phép" trong SharePoint điều này có thể liên quan đến việc bỏ dùng TLS 1.0/1.1. Để biết thêm thông tin, hãy xem:

[Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Lỗi xác thực xảy ra nếu máy khách không có hỗ trợ TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Nếu người dùng đang sử Windows 7, hãy đảm bảo họ đánh dấu chọn [TLS Cipher Suites trong Windows 7.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)