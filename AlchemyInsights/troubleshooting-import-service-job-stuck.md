---
title: Khắc phục sự cố kẹt Công việc Dịch vụ Nhập
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125776"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Khắc phục sự cố kẹt Công việc Dịch vụ Nhập

Nếu bạn đang gặp sự cố khi nhập công việc dịch vụ bị kẹt hoặc gặp thất bại, hãy kiểm tra và thử các cách sau:

- Xem lại kích cỡ tệp PST. Kích cỡ tối đa được đề xuất của tệp PST để nhập là 20 GB.

- Nếu bạn nghi ngờ các mục bị bỏ qua do hỏng, hãy chạy Scanpst.exe đoán và khắc phục lỗi trong tệp PST.

- Nếu bạn thấy lỗi "MapiExceptionShutoffQuotaExceeded" trong khi nhập, hãy đảm bảo hộp thư đích có đủ khả năng để nhập các tệp PST mong muốn.

Để biết thêm thông tin về cách khắc phục sự cố công việc nhập PST, hãy xem [Khắc phục sự cố với công việc nhập PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Để biết thông tin về cách khắc phục sự cố khi nhập PST vào Outlook, hãy xem khắc phục sự cố khi nhập tệp [Outlook .pst (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)