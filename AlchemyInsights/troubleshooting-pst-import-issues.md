---
title: Khắc phục sự cố PST nhập khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991388"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="65643-102">Khắc phục sự cố PST nhập khẩu</span><span class="sxs-lookup"><span data-stu-id="65643-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="65643-103">Nếu bạn đang nhập khẩu trong máy khách Outlook chính nó, hãy xem [khắc phục sự cố nhập tệp. PST Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="65643-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="65643-104">Nếu bạn đang sử dụng dịch vụ nhập và nó bị kẹt, xin lưu ý rằng mỗi tệp PST mà bạn tải lên vị trí lưu trữ Azure sẽ không lớn hơn 20 GB.</span><span class="sxs-lookup"><span data-stu-id="65643-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="65643-105">PST các tập tin lớn hơn 20 GB có thể ảnh hưởng đến hiệu suất của quá trình PST nhập khẩu.</span><span class="sxs-lookup"><span data-stu-id="65643-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="65643-106">Nếu bạn muốn kiểm tra trạng thái của một công việc nhập cụ thể, bạn có thể sử dụng [Get-MailboxImportRequest-batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="65643-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="65643-107">Để biết chi tiết đầy đủ về các dịch vụ nhập khẩu, xin vui lòng xem [tổng quan về nhập khẩu của tổ chức của bạn PST tập tin](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="65643-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
