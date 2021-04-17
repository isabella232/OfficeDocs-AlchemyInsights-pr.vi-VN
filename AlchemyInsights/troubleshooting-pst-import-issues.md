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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="a504a-102">Khắc phục sự cố PST nhập vấn đề</span><span class="sxs-lookup"><span data-stu-id="a504a-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="a504a-103">Nếu bạn đang nhập trong ứng dụng khách Outlook chính nó, vui lòng xem [khắc phục sự cố khi nhập tệp Outlook. PST](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="a504a-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="a504a-104">Nếu bạn đang sử dụng dịch vụ nhập và nó bị kẹt, vui lòng lưu ý rằng mỗi tệp PST mà bạn tải lên đến vị trí lưu trữ Azure sẽ không lớn hơn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="a504a-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="a504a-105">PST các tệp lớn hơn 20 GB có thể ảnh hưởng đến hiệu suất của quy trình nhập PST.</span><span class="sxs-lookup"><span data-stu-id="a504a-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="a504a-106">Nếu bạn muốn xác minh trạng thái của một công việc nhập cụ thể, bạn có thể dùng [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="a504a-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="a504a-107">Để biết chi tiết đầy đủ về dịch vụ nhập, vui lòng xem [tổng quan về việc nhập các TỆP PST của tổ chức của bạn](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="a504a-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
