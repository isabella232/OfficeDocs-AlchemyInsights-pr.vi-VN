---
title: Chặn tải xuống trên các liên kết chia sẻ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000213"
- "5715"
ms.openlocfilehash: 8cb53754125cedf4a3d0426d6c3bf70297eb3d74
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358508"
---
# <a name="block-download-on-sharing-links"></a><span data-ttu-id="39156-102">Chặn tải xuống trên các liên kết chia sẻ</span><span class="sxs-lookup"><span data-stu-id="39156-102">Block download on sharing links</span></span>

<span data-ttu-id="39156-103">**Chặn tải** có sẵn để **xem chỉ liên kết** đến tài liệu Office.</span><span class="sxs-lookup"><span data-stu-id="39156-103">**Block download** is available for **view-only links** to Office documents.</span></span> <span data-ttu-id="39156-104">Khi bạn chọn tùy chọn này, những người có quyền truy cập vào tệp qua liên kết bạn tạo sẽ không thấy các tùy chọn để tải xuống, in hoặc sao chép tệp.</span><span class="sxs-lookup"><span data-stu-id="39156-104">When you select this option, people who gain access to the file via the link you created will not see options to download, print, or copy the file.</span></span>

<span data-ttu-id="39156-105">Quản trị viên có thể kiểm soát xem cài đặt "chặn tải xuống" chỉ xuất hiện cho tệp Office hay không bằng cách thay đổi `BlockDownloadLinksFileType` thiết đặt trong lệnh ghép ngắn [Set-spothuê](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) hoặc [thiết lập sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell.</span><span class="sxs-lookup"><span data-stu-id="39156-105">Administrators can control whether the "block download" setting appears only for Office files or not by changing the `BlockDownloadLinksFileType` setting in the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/set-spotenant?view=sharepoint-ps) or [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) PowerShell cmdlets.</span></span>
