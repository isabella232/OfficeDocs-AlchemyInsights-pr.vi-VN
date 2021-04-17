---
title: Khắc phục sự cố PST nhập vấn đề
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
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826185"
---
# <a name="troubleshooting-pst-import-issues"></a>Khắc phục sự cố PST nhập vấn đề

- Nếu bạn đang nhập trong ứng dụng khách Outlook chính nó, vui lòng xem [khắc phục sự cố khi nhập tệp Outlook. PST](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Nếu bạn đang sử dụng dịch vụ nhập và nó bị kẹt, vui lòng lưu ý rằng mỗi tệp PST mà bạn tải lên đến vị trí lưu trữ Azure sẽ không lớn hơn 20 GB. PST các tệp lớn hơn 20 GB có thể ảnh hưởng đến hiệu suất của quy trình nhập PST.

- Nếu bạn muốn xác minh trạng thái của một công việc nhập cụ thể, bạn có thể dùng [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Để biết chi tiết đầy đủ về dịch vụ nhập, vui lòng xem [tổng quan về việc nhập các TỆP PST của tổ chức của bạn](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
