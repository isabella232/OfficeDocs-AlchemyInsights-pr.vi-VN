---
title: 726 chặn chuyển tiếp email
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219877"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="425bf-102">Chặn hoặc bỏ chặn chuyển tiếp email</span><span class="sxs-lookup"><span data-stu-id="425bf-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="425bf-103">Để bật hoặc tắt tính năng chuyển tiếp email cho một hộp thư cụ thể, hãy xem mục [đặt cấu hình chuyển tiếp email](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="425bf-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="425bf-104">Trên mức đối tượng thuê, kiểm soát việc chuyển tiếp bên ngoài được thực hiện bằng cách sử dụng chính sách chống thư rác đi.</span><span class="sxs-lookup"><span data-stu-id="425bf-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="425bf-105">Nếu nó được đặt là tắt hoặc tự động, có thể chặn chuyển tiếp email với truy nhập "550 5.7.520 bị từ chối, tổ chức của bạn không cho phép" chuyển tiếp ngoài ".</span><span class="sxs-lookup"><span data-stu-id="425bf-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="425bf-106">Sau đó, nếu chuyển tiếp đã được thiết lập để bị chặn, đó là lỗi người dùng của bạn sẽ thấy.</span><span class="sxs-lookup"><span data-stu-id="425bf-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="425bf-107">Nếu việc chuyển tiếp bị chặn, hãy đảm bảo rằng chính sách được cấu hình để bật tự động chuyển tiếp bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="425bf-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="425bf-108">Bạn có thể kiểm tra chính sách lọc thư rác từ Trung tâm bảo mật và tuân thủ hoặc bằng cách chạy lệnh Get-Hosteioutboundspamfilterpolicy | FL name, tự động chuyển sang chế độ.</span><span class="sxs-lookup"><span data-stu-id="425bf-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="425bf-109">Nếu bạn muốn thiết lập khóa tự động chuyển tiếp, lệnh đó sẽ cho bạn biết trạng thái chính sách ngay bây giờ.</span><span class="sxs-lookup"><span data-stu-id="425bf-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="425bf-110">Lưu ý: chúng tôi khuyên bạn nên giữ tự động bị vô hiệu hóa ở bên ngoài trong chính sách bộ lọc thư rác mặc định của bạn và chỉ cho phép những người dùng cần chuyển tiếp bên ngoài bằng cách tạo chính sách tùy chỉnh cho những người dùng đó.</span><span class="sxs-lookup"><span data-stu-id="425bf-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="425bf-111">Bạn có thể đọc thêm trong [cấu hình chuyển tiếp email bên ngoài trong Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="425bf-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>