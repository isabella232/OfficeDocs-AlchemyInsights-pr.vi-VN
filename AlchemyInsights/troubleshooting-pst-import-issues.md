---
title: Khắc phục sự cố nhập PST
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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972441"
---
# <a name="troubleshooting-pst-import-issues"></a>Khắc phục sự cố nhập PST

- Nếu bạn đang nhập trong phạm vi toàn Outlook máy khách, hãy xem khắc phục sự cố khi [nhập Outlook tệp .pst](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Nếu bạn đang sử dụng Dịch vụ Nhập và gặp sự cố, hãy lưu ý rằng mỗi tệp PST mà bạn tải lên vị trí Lưu trữ Azure không được lớn hơn 20 GB. Tệp PST lớn hơn 20GB có thể ảnh hưởng đến hiệu suất của quy trình nhập PST. Để biết thêm thông tin về cách khắc phục sự cố các công việc [bị kẹt, hãy xem Các sự cố ảnh hưởng đến công việc nhập PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Nếu bạn muốn xác minh trạng thái của một công việc Nhập cụ thể, hãy sử [dụng Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Để biết chi tiết đầy đủ về dịch vụ nhập, [hãy xem Tổng quan về việc nhập tệp PST của tổ chức bạn.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
