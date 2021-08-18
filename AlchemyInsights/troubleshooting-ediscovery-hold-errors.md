---
title: Khắc phục sự cố khám phá chứa lỗi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 70f0302fd13324b6778390aeb0fe41ff5668d0d1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330802"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Khắc phục sự cố khám phá chứa lỗi

Bạn gặp phải sự cố với việc lưu giữ Khám phá Điện tử? Dưới đây là một số cách thực hành tốt nhất cần xem xét:

- Kiểm tra trạng thái phân phối giữ lại.  Nếu trạng thái là **Bật (Đang chờ)** hoặc **Tắt (Đang chờ xử lý),** hãy chờ phân phối giữ để hoàn tất.
- Phối Khám phá Điện tử lưu giữ các bản cập nhật thành một yêu cầu hàng loạt duy nhất thay vì cập nhật chính sách nhiều lần cho mỗi giao dịch.
- Chạy Set-CaseHoldPolicy <policyname> -RetryDistribution trong Powershell của Trung tâm Bảo mật và Tuân thủ. Để biết chi tiết, hãy [Kết nối xem Trung tâm Bảo & Tuân thủ PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell).

Để biết các bước kiểm tra các thiết đặt này và các cách thực hành tốt nhất khác để giảm thiểu và giải quyết vấn đề giữ Lại Khám phá Điện [tử,](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors)hãy xem Khắc phục sự cố lỗi giữ Khám phá Điện tử .
Để biết thông tin về cách khắc phục các sự cố Khám phá Điện tử phổ biến khác, hãy xem điều tra, khắc phục sự cố và giải quyết các [sự cố Thường gặp về Khám phá Điện tử.](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
