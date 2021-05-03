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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="38b29-102">Sự cố với SharePoint trên Windows 7 máy</span><span class="sxs-lookup"><span data-stu-id="38b29-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="38b29-103">Nếu bạn nhận được lỗi trên máy Windows 7 trong khi làm việc trên SharePoint hoặc OneDrive, chúng có thể liên quan đến việc TLS 1.0/1 bị bỏ dùng.</span><span class="sxs-lookup"><span data-stu-id="38b29-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="38b29-104">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="38b29-104">For more information, see:</span></span>

- [<span data-ttu-id="38b29-105">Chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="38b29-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="38b29-106">Windows khách 7 SP1/Windows 8 khách phải được bật TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="38b29-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="38b29-107">Để biết thêm thông tin, [hãy xem mục Lỗi xác thực xảy ra khi máy khách không có hỗ trợ TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="38b29-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="38b29-108">Cài đặt KB3140245 và tạo giá trị sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="38b29-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="38b29-109">Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) làm giao thức bảo mật mặc định trong WinHTTP trong Windows</span><span class="sxs-lookup"><span data-stu-id="38b29-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="38b29-110">Windows khách 7 SP1/Windows 8 phải đảm bảo cài đặt bộ mã VLS mới nhất.</span><span class="sxs-lookup"><span data-stu-id="38b29-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="38b29-111">Để biết thêm thông tin, [hãy xem mục Tư vấn Bảo mật Microsoft 3042058.](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058)</span><span class="sxs-lookup"><span data-stu-id="38b29-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


