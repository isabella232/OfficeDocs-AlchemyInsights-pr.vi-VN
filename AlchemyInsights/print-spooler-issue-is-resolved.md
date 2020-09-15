---
title: Khắc phục sự cố bộ đệm in được giải quyết
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 66b39434ef6f9ad2b8392f811704e67c1bcffd2b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801863"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="24874-102">Khắc phục sự cố bộ đệm in được giải quyết</span><span class="sxs-lookup"><span data-stu-id="24874-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="24874-103">Nếu thiết bị của bạn đã được Cập Nhật với Windows 10  **OS bản dựng 19041,329**, bạn có thể đã quan sát sự cố khi in một số máy in nào đó.</span><span class="sxs-lookup"><span data-stu-id="24874-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="24874-104">Bộ đệm in có thể ném lỗi hoặc đóng đột ngột khi tìm cách in và không có đầu ra từ máy in bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="24874-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="24874-105">Sự cố này được giải quyết trong hệ điều hành bản dựng  **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="24874-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="24874-106">**Điều tra liên tục**</span><span class="sxs-lookup"><span data-stu-id="24874-106">**Ongoing investigation**</span></span>

<span data-ttu-id="24874-107">Tệp dịch vụ hệ thống con cố định cục bộ bảo mật cục bộ (LSASS) (**Isass.exe**) có thể không thành công trong một số thiết bị có thông báo lỗi, "quy trình hệ thống quan trọng, C:\WINDOWS\system32\Isass.exe, không thành công với mã trạng thái c0000008.</span><span class="sxs-lookup"><span data-stu-id="24874-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="24874-108">Giờ đây, máy phải được khởi động lại ".</span><span class="sxs-lookup"><span data-stu-id="24874-108">The machine must now be restarted".</span></span>  <span data-ttu-id="24874-109">**Microsoft đang làm việc với độ phân giải và sẽ cung cấp bản Cập Nhật trong bản phát hành sắp tới.**</span><span class="sxs-lookup"><span data-stu-id="24874-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="24874-110">Để biết thêm thông tin, vui lòng kiểm tra  [Windows 10 phiên bản 2004 đã biết sự cố](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="24874-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>