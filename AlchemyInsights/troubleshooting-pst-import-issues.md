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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059837"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="c93c7-102">Khắc phục sự cố nhập PST</span><span class="sxs-lookup"><span data-stu-id="c93c7-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="c93c7-103">Nếu bạn đang nhập từ chính máy khách Outlook đó, hãy xem mục Khắc [phục sự cố khi nhập tệp .pst của Outlook.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)</span><span class="sxs-lookup"><span data-stu-id="c93c7-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="c93c7-104">Nếu bạn đang sử dụng Dịch vụ Nhập và gặp sự cố, hãy lưu ý rằng mỗi tệp PST mà bạn tải lên vị trí Lưu trữ Azure không được lớn hơn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="c93c7-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="c93c7-105">Tệp PST lớn hơn 20GB có thể ảnh hưởng đến hiệu suất của quy trình nhập PST.</span><span class="sxs-lookup"><span data-stu-id="c93c7-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="c93c7-106">Để biết thêm thông tin về cách khắc phục sự cố các công việc [bị kẹt, hãy xem Các sự cố ảnh hưởng đến công việc nhập PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="c93c7-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="c93c7-107">Nếu bạn muốn xác minh trạng thái của một công việc Nhập cụ thể, hãy sử [dụng Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="c93c7-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="c93c7-108">Để biết chi tiết đầy đủ về dịch vụ nhập, [hãy xem Tổng quan về việc nhập tệp PST của tổ chức bạn.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="c93c7-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
