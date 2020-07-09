---
title: Vấn đề bộ đệm in được giải quyết
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088530"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="21d82-102">Vấn đề bộ đệm in được giải quyết</span><span class="sxs-lookup"><span data-stu-id="21d82-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="21d82-103">Nếu thiết bị của bạn đã được Cập Nhật với Windows 10 **OS Build 19041,329**, bạn có thể đã quan sát thấy sự cố trong đó một số máy in không in được.</span><span class="sxs-lookup"><span data-stu-id="21d82-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="21d82-104">Bộ đệm in có thể ném một lỗi hoặc đóng đột ngột khi cố gắng in và không có kết quả đến từ máy in bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="21d82-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="21d82-105">Vấn đề này được giải quyết trong HĐH bản dựng **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="21d82-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="21d82-106">**Điều tra liên tục**</span><span class="sxs-lookup"><span data-stu-id="21d82-106">**Ongoing investigation**</span></span>

<span data-ttu-id="21d82-107">Tệp cục bộ bảo mật quyền subsystem Service (LSASS) (**Isass.exe**) có thể không thành công trên một số thiết bị có thông báo lỗi "quá trình hệ thống quan trọng, C:\WINDOWS\system32\Isass.exe, thất bại với mã trạng thái c0000008.</span><span class="sxs-lookup"><span data-stu-id="21d82-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="21d82-108">Máy bây giờ phải được khởi động lại ".</span><span class="sxs-lookup"><span data-stu-id="21d82-108">The machine must now be restarted".</span></span>  <span data-ttu-id="21d82-109">**Microsoft đang làm việc trên một độ phân giải và sẽ cung cấp một bản Cập Nhật trong một bản phát hành sắp tới.**</span><span class="sxs-lookup"><span data-stu-id="21d82-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="21d82-110">Để biết thêm thông tin, hãy kiểm tra [Phiên bản Windows 10 2004 vấn đề đã biết](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="21d82-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>