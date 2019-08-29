---
title: Chuyển tiếp email thông qua Office 365
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
ms.openlocfilehash: ffdaca1ba45a6f273809dbe50a7c40e8610193e1
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666538"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="1e459-102">Thiết lập một thiết bị đa chức năng hoặc ứng dụng để gửi email bằng cách sử dụng Office 365</span><span class="sxs-lookup"><span data-stu-id="1e459-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="1e459-103">Để tìm hiểu về lựa chọn của bạn và các bước, hãy xem [làm thế nào để thiết lập một thiết bị đa chức năng hoặc ứng dụng để gửi email bằng cách sử dụng Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="1e459-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="1e459-104">**Lưu ý:** Nếu bạn có một thiết bị hoặc ứng dụng mới ngừng làm việc, xin vui lòng lưu ý chúng tôi mới bắt đầu [vô hiệu hóa mã 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) theo kế hoạch.</span><span class="sxs-lookup"><span data-stu-id="1e459-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="1e459-105">Để xem các thiết bị bị ảnh hưởng, đi đến [SMTP Auth khách hàng báo cáo](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="1e459-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="1e459-106">Lỗi phổ biến có thể là tương tự như: lỗi thất bại xác thực, TLS không/lỗi, thuật toán mật mã lỗi, thuật toán mismatch hoặc kết nối giảm xuống.</span><span class="sxs-lookup"><span data-stu-id="1e459-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="1e459-107">Để giải quyết vấn đề:</span><span class="sxs-lookup"><span data-stu-id="1e459-107">To resolve the issue:</span></span>
 - <span data-ttu-id="1e459-108">**Windows Server 2003 IIS SMTP sẽ không còn làm việc-một phiên bản mới hơn của Windows là cần thiết.**</span><span class="sxs-lookup"><span data-stu-id="1e459-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="1e459-109">Xin vui lòng kiểm tra với đại lý ứng dụng hoặc thiết bị của bạn để xem nếu một thuật toán mật mã hiện đại được hỗ trợ, hoặc nếu có một Cập Nhật.</span><span class="sxs-lookup"><span data-stu-id="1e459-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
