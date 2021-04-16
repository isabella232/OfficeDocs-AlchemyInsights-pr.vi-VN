---
title: Chuyển tiếp email qua Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 56936541c52e56d7aa9b0f5dad7b9a359c5b6185
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809677"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="6653c-102">Thiết lập thiết bị đa năng hoặc ứng dụng để gửi email</span><span class="sxs-lookup"><span data-stu-id="6653c-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="6653c-103">Để tìm hiểu về các tùy chọn của bạn và các bước, hãy xem [cách thiết lập thiết bị đa năng hoặc ứng dụng để gửi email bằng Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="6653c-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="6653c-104">**Lưu ý:** Nếu bạn có một thiết bị hoặc ứng dụng đã ngừng hoạt động gần đây, vui lòng lưu ý rằng chúng tôi đã bắt đầu tắt tính năng ký [hiệu 3DES](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) như đã lên kế hoạch.</span><span class="sxs-lookup"><span data-stu-id="6653c-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="6653c-105">Để xem các thiết bị bị ảnh hưởng, hãy đi đến [báo cáo khách hàng của SMTP Auth](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="6653c-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="6653c-106">Các lỗi thông thường có thể tương tự như: lỗi xác thực/lỗi, lỗi TLS/lỗi, thuật toán mật mã lỗi, thuật toán không khớp hoặc kết nối bị bỏ.</span><span class="sxs-lookup"><span data-stu-id="6653c-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="6653c-107">Để giải quyết sự cố:</span><span class="sxs-lookup"><span data-stu-id="6653c-107">To resolve the issue:</span></span>

 - <span data-ttu-id="6653c-108">**Windows Server 2003 IIS SMTP sẽ không còn hoạt động – phiên bản Windows mới hơn.**</span><span class="sxs-lookup"><span data-stu-id="6653c-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="6653c-109">Vui lòng kiểm tra với ứng dụng hoặc nhà cung cấp thiết bị của bạn để xem có một mật mã hiện đại được hỗ trợ hay không nếu có bản Cập Nhật hay không.</span><span class="sxs-lookup"><span data-stu-id="6653c-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
