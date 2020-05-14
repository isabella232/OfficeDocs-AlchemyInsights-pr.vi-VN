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
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/13/2020
ms.locfileid: "43785217"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="a07ed-102">Thiết lập thiết bị hoặc ứng dụng đa chức năng để gửi email</span><span class="sxs-lookup"><span data-stu-id="a07ed-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="a07ed-103">Để tìm hiểu về các tùy chọn của bạn và các bước, hãy xem [cách thiết lập thiết bị hoặc ứng dụng đa chức năng để gửi email bằng cách sử dụng Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="a07ed-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="a07ed-104">**Lưu ý:** Nếu bạn có một thiết bị hoặc ứng dụng mà gần đây đã ngừng làm việc, xin lưu ý chúng tôi gần đây đã bắt đầu [vô hiệu hóa các 3DES mật mã](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) theo kế hoạch.</span><span class="sxs-lookup"><span data-stu-id="a07ed-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="a07ed-105">Để xem các thiết bị bị ảnh hưởng, hãy truy cập [báo cáo smtp auth khách hàng](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="a07ed-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="a07ed-106">Lỗi phổ biến có thể tương tự như: lỗi xác thực/sai, TLS lỗi/sai, thuật toán mật mã lỗi, thuật toán không phù hợp, hoặc kết nối giảm xuống.</span><span class="sxs-lookup"><span data-stu-id="a07ed-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="a07ed-107">Để khắc phục sự cố:</span><span class="sxs-lookup"><span data-stu-id="a07ed-107">To resolve the issue:</span></span>
 - <span data-ttu-id="a07ed-108">**Windows Server 2003 IIS SMTP sẽ không còn hoạt động – một phiên bản mới hơn của Windows là bắt buộc.**</span><span class="sxs-lookup"><span data-stu-id="a07ed-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="a07ed-109">Vui lòng kiểm tra với nhà cung cấp thiết bị hoặc ứng dụng của bạn để xem liệu mật mã hiện đại có được hỗ trợ hay không hoặc nếu có bản Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="a07ed-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
