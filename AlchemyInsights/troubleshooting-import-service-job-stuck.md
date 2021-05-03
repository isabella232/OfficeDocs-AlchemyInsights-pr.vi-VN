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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="5e538-102">Khắc phục sự cố kẹt Công việc Dịch vụ Nhập</span><span class="sxs-lookup"><span data-stu-id="5e538-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="5e538-103">Nếu bạn đang gặp sự cố khi nhập công việc dịch vụ bị kẹt hoặc gặp thất bại, hãy kiểm tra và thử các cách sau:</span><span class="sxs-lookup"><span data-stu-id="5e538-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="5e538-104">Xem lại kích cỡ tệp PST.</span><span class="sxs-lookup"><span data-stu-id="5e538-104">Review the size of of the PST file.</span></span> <span data-ttu-id="5e538-105">Kích cỡ tối đa được đề xuất của tệp PST để nhập là 20 GB.</span><span class="sxs-lookup"><span data-stu-id="5e538-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="5e538-106">Nếu bạn nghi ngờ các mục bị bỏ qua do hỏng, hãy chạy Scanpst.exe đoán và khắc phục lỗi trong tệp PST.</span><span class="sxs-lookup"><span data-stu-id="5e538-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="5e538-107">Nếu bạn thấy lỗi "MapiExceptionShutoffQuotaExceeded" trong khi nhập, hãy đảm bảo hộp thư đích có đủ khả năng để nhập các tệp PST mong muốn.</span><span class="sxs-lookup"><span data-stu-id="5e538-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="5e538-108">Để biết thêm thông tin về cách khắc phục sự cố công việc nhập PST, hãy xem [Khắc phục sự cố với công việc nhập PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="5e538-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="5e538-109">Để biết thông tin về cách khắc phục sự cố khi nhập PST vào Outlook, hãy xem khắc phục sự cố khi nhập tệp [Outlook .pst (microsoft.com).](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="5e538-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>