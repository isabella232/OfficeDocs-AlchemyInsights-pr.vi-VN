---
title: S/MIME trong Outlook trên web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053247"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="dac27-102">Mã hóa thư email trong Outlook</span><span class="sxs-lookup"><span data-stu-id="dac27-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="dac27-103">Văn phòng 365 mã hóa thư được xây dựng trên Microsoft Azure quyền quản lý (Azure RMS), là một phần của Azure bảo vệ thông tin.</span><span class="sxs-lookup"><span data-stu-id="dac27-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="dac27-104">Nếu đăng ký của bạn bao gồm quản lý quyền Azure hoặc bảo vệ thông tin Azure, **bạn không cần thực hiện bất kỳ hành động nào để bật hoặc kích hoạt** dịch vụ quản lý quyền theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="dac27-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="dac27-105">Dựa trên phản hồi của khách hàng, chúng tôi sẽ không còn kích hoạt quy tắc luồng thư Exchange để tự động mã hóa email gửi đi có chứa một loại thông tin nhạy cảm nhất định trong đối tượng thuê của bạn theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="dac27-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="dac27-106">Thay vào đó, chúng tôi đang cung cấp hướng dẫn chi tiết về cách bạn có thể làm như vậy mình.</span><span class="sxs-lookup"><span data-stu-id="dac27-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="dac27-107">Để biết thêm chi tiết về cách tạo quy tắc truyền tải để mã hóa thông tin nhạy cảm, xem [bài viết này](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="dac27-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="dac27-108">Nếu sử dụng Outlook trên web (trước đây là **OWA**): khi soạn thư email, chỉ cần bấm **bảo vệ** trong OWA.</span><span class="sxs-lookup"><span data-stu-id="dac27-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="dac27-109">Điều này sẽ áp dụng cho phép "không chuyển tiếp".</span><span class="sxs-lookup"><span data-stu-id="dac27-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="dac27-110">Nhấp vào **thay đổi quyền** và chọn **mã hóa** chỉ để mã hóa thư.</span><span class="sxs-lookup"><span data-stu-id="dac27-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="dac27-111">Nếu sử dụng **máy khách Outlook**: để gửi một tin nhắn được mã hóa từ Outlook 2013 hoặc 2016, hoặc Outlook 2016 cho Mac, chọn **tùy chọn** > **quyền**, sau đó chọn tùy chọn bảo vệ bạn cần.</span><span class="sxs-lookup"><span data-stu-id="dac27-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="dac27-112">Để **tự động mã hóa tất cả email** được gửi đến người nhận nhất định hoặc các tổ chức đối tác bên ngoài, bạn cần tạo quy tắc truyền tải luồng thư trong Trung tâm quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="dac27-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="dac27-113">Hướng dẫn chi tiết được cung cấp trong [bài viết hỗ trợ này](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="dac27-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

