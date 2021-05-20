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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539954"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="52f47-102">401 Lỗi trái phép trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="52f47-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="52f47-103">Nếu bạn nhận được lỗi "(401) Trái phép" trong SharePoint điều này có thể liên quan đến việc bỏ dùng TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="52f47-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="52f47-104">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="52f47-104">For more info, see:</span></span>

- [<span data-ttu-id="52f47-105">Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="52f47-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="52f47-106">Lỗi xác thực xảy ra nếu máy khách không có hỗ trợ TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="52f47-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="52f47-107">Cập nhật để bật TLS 1.1 và TLS 1.2 làm giao thức bảo mật mặc định trong WinHTTP trong Windows</span><span class="sxs-lookup"><span data-stu-id="52f47-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="52f47-108">Nếu người dùng đang sử Windows 7, hãy đảm bảo họ đánh dấu chọn [TLS Cipher Suites trong Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="52f47-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>