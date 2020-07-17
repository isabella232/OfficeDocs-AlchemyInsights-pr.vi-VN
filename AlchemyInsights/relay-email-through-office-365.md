---
title: Chuyển tiếp email thông qua Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 074a9106553bf3a2a5e563f9ebaca9dfc38111cb
ms.sourcegitcommit: 9872280f71429d2344b0b441e218fba5b3bd3cf7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/02/2020
ms.locfileid: "45023481"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="5bda7-102">Thiết lập thiết bị hoặc ứng dụng đa chức năng để gửi email</span><span class="sxs-lookup"><span data-stu-id="5bda7-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="5bda7-103">Để tìm hiểu về các tùy chọn của bạn và các bước, hãy xem [cách thiết lập thiết bị hoặc ứng dụng đa chức năng để gửi email bằng cách sử dụng Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="5bda7-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="5bda7-104">**Lưu ý:** Nếu bạn có một thiết bị hoặc ứng dụng mà gần đây đã ngừng làm việc, xin lưu ý chúng tôi gần đây đã bắt đầu [vô hiệu hóa các 3DES mật mã](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) theo kế hoạch.</span><span class="sxs-lookup"><span data-stu-id="5bda7-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="5bda7-105">Để xem các thiết bị bị ảnh hưởng, hãy truy cập [báo cáo smtp auth khách hàng](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="5bda7-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="5bda7-106">Lỗi phổ biến có thể tương tự như: lỗi xác thực/sai, TLS lỗi/sai, thuật toán mật mã lỗi, thuật toán không phù hợp, hoặc kết nối giảm xuống.</span><span class="sxs-lookup"><span data-stu-id="5bda7-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="5bda7-107">Để khắc phục sự cố:</span><span class="sxs-lookup"><span data-stu-id="5bda7-107">To resolve the issue:</span></span>

 - <span data-ttu-id="5bda7-108">**Windows Server 2003 IIS SMTP sẽ không còn hoạt động – một phiên bản mới hơn của Windows là bắt buộc.**</span><span class="sxs-lookup"><span data-stu-id="5bda7-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="5bda7-109">Vui lòng kiểm tra với nhà cung cấp thiết bị hoặc ứng dụng của bạn để xem liệu mật mã hiện đại có được hỗ trợ hay không hoặc nếu có bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="5bda7-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
