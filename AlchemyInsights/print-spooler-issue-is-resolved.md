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
# <a name="print-spooler-issue-is-resolved"></a>Vấn đề bộ đệm in được giải quyết

Nếu thiết bị của bạn đã được Cập Nhật với Windows 10 **OS Build 19041,329**, bạn có thể đã quan sát thấy sự cố trong đó một số máy in không in được. Bộ đệm in có thể ném một lỗi hoặc đóng đột ngột khi cố gắng in và không có kết quả đến từ máy in bị ảnh hưởng. Vấn đề này được giải quyết trong HĐH bản dựng **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).  

**Điều tra liên tục**

Tệp cục bộ bảo mật quyền subsystem Service (LSASS) (**Isass.exe**) có thể không thành công trên một số thiết bị có thông báo lỗi "quá trình hệ thống quan trọng, C:\WINDOWS\system32\Isass.exe, thất bại với mã trạng thái c0000008. Máy bây giờ phải được khởi động lại ".  **Microsoft đang làm việc trên một độ phân giải và sẽ cung cấp một bản Cập Nhật trong một bản phát hành sắp tới.**

Để biết thêm thông tin, hãy kiểm tra [Phiên bản Windows 10 2004 vấn đề đã biết](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).