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
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53118005"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="56f6d-102">Thiết lập ứng dụng hoặc thiết bị đa năng để gửi email</span><span class="sxs-lookup"><span data-stu-id="56f6d-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="56f6d-103">Để tìm hiểu về các tùy chọn và các bước, xem mục Cách thiết lập thiết bị đa năng hoặc ứng dụng để [gửi email bằng](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="56f6d-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="56f6d-104">Nếu bạn có một thiết bị hoặc ứng dụng mà gần đây đã ngừng hoạt động, các vấn đề phổ biến nhất là:</span><span class="sxs-lookup"><span data-stu-id="56f6d-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="56f6d-105">**Xác thực các lỗi liên quan đến xác thực trong khi sử dụng bản gửi máy khách SmTP Auth** Gần đây, chúng tôi đã thực hiện một số thay đổi liên quan đến cách thức hoạt động của Xác thực SMTP.</span><span class="sxs-lookup"><span data-stu-id="56f6d-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="56f6d-106">Để biết thêm thông tin về cách giải quyết sự cố, hãy xem mục xác thực không thành công trong mục Khắc phục sự cố với máy in, máy quét và ứng dụng LOB gửi email bằng Microsoft 365 hoặc [máy Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)</span><span class="sxs-lookup"><span data-stu-id="56f6d-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="56f6d-107">**Chúng tôi chỉ chấp nhận phiên bản TLS 1.2 trong khi tạo kết nối bảo mật để truy Office 365** Nếu bạn đang sử dụng Kết nối bảo mật (TLS), hãy đảm bảo thiết bị ứng dụng của bạn hỗ trợ TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="56f6d-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="56f6d-108">Để biết thêm thông tin, [hãy xem chuẩn bị cho TLS 1.2 trong Office 365 và Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="56f6d-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="56f6d-109">Để biết các sự cố và giải pháp khác, hãy xem mục Khắc phục sự cố với máy in, máy quét và các ứng dụng LOB gửi email bằng Microsoft 365 hoặc [Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="56f6d-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="56f6d-110">Để xem các thiết bị bị ảnh hưởng, hãy đi đến [báo cáo Máy khách Xác thực SMTP.](https://protection.office.com/mailflow/dashboard)</span><span class="sxs-lookup"><span data-stu-id="56f6d-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="56f6d-111">**Lưu** ý : Exchange Online không phù hợp với tình huống gửi thư hàng loạt.</span><span class="sxs-lookup"><span data-stu-id="56f6d-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="56f6d-112">Để gửi email thương mại hàng loạt (ví dụ: bản tin khách hàng), bạn nên sử dụng các nhà cung cấp bên thứ ba chuyên về các dịch vụ này.</span><span class="sxs-lookup"><span data-stu-id="56f6d-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
