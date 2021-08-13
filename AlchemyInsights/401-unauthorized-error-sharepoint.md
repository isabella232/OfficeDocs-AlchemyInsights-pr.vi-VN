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
ms.openlocfilehash: 3b81bab22c9deb6498827b01f54fac0be2f7c35b6f912d729b44ddc4f45598cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919049"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Lỗi trái phép trong SharePoint

Nếu bạn nhận được lỗi "(401) Trái phép" trong SharePoint điều này có thể liên quan đến việc bỏ dùng TLS 1.0/1.1. Để biết thêm thông tin, hãy xem:

- [Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Lỗi xác thực xảy ra nếu máy khách không có hỗ trợ TLS 1.2](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Cập nhật để bật TLS 1.1 và TLS 1.2 làm giao thức bảo mật mặc định trong WinHTTP trong Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Nếu người dùng đang sử Windows 7, hãy đảm bảo họ đánh dấu chọn [TLS Cipher Suites trong Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)