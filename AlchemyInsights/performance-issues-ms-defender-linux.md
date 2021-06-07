---
title: Sự cố về hiệu suất đối với Microsoft Defender dành cho Điểm cuối trên Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794221"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Sự cố về hiệu suất đối với Microsoft Defender dành cho Điểm cuối trên Linux

Bài viết này hướng dẫn bạn qua các bước xác định sự cố hiệu suất cho Microsoft Defender dành cho Điểm cuối trên Linux.

Điều quan trọng là trước tiên phải xác minh rằng vấn đề mà bạn đang gặp phải được giải quyết bằng phiên [bản mới nhất.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Để bắt đầu điều tra, hãy xem mục [Khắc phục sự cố về hiệu suất cho Microsoft Defender dành cho Điểm cuối trên Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).

## <a name="exclusions"></a>Loại trừ

Loại trừ có thể giúp giảm thiểu sự cố về hiệu suất. Hãy xem lại các mục loại trừ trước khi bắt đầu để biết và ghi nhận mọi rủi ro bổ sung.

Để biết thêm thông tin, hãy xem mục Đặt cấu hình và xác thực các mục loại trừ [cho Bộ bảo vệ Microsoft dành cho Điểm cuối trên Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Khi bạn có nhiều tệp và & mục cần loại trừ và tất cả đều nằm ở cùng một điểm gắn kết, việc loại trừ điểm gắn có có thể sẽ dễ dàng hơn. Bắt đầu từ bản phát hành Tháng Hai 101.22.80, bạn có thể loại trừ toàn bộ điểm gắn kết.

Ví dụ: nếu /mnt/backup là một mountpoint, bạn có thể thêm /mnt/backup vào danh sách loại trừ bằng cách chạy lệnh này:

`$ mdatp exclusion folder add –path /mnt/backup`

**Lưu** ý: Việc thêm loại trừ sẽ làm tăng nguy cơ không phát hiện phần mềm xấu, đồng thời cần được xử lý và thực hiện một cách cẩn thận.

## <a name="need-help"></a>Bạn cần Trợ giúp?

Để hỗ trợ bạn một cách hiệu quả nhất, hãy thu thập dữ liệu chẩn đoán trước khi mở một trường hợp hỗ trợ.
