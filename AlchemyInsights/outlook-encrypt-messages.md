---
title: S/MIME trong Outlook trên web
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772320"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="fdbe6-102">Mã hóa thư email trong Outlook</span><span class="sxs-lookup"><span data-stu-id="fdbe6-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="fdbe6-103">Mã hóa thư Microsoft 365 được xây dựng trên Microsoft Azure Rights Management (Azure RMS), là một phần trong bảo vệ thông tin Azure.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="fdbe6-104">Nếu thuê bao của bạn bao gồm Azure rights management hoặc Azure Information Protection, **bạn không cần phải thực hiện bất kỳ hành động nào để bật hoặc kích hoạt** dịch vụ quản lý quyền theo cách thủ công.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="fdbe6-105">Dựa trên phản hồi của khách hàng, chúng tôi sẽ không còn cho phép các quy tắc dòng thư Exchange để tự động mã hóa email có chứa một số loại thông tin nhạy cảm trong đối tượng thuê của bạn theo mặc định.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="fdbe6-106">Thay vào đó, chúng tôi đang cung cấp các hướng dẫn chi tiết về cách bạn có thể làm như vậy.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="fdbe6-107">Để biết thêm chi tiết về cách tạo quy tắc truyền dẫn để mã hóa thông tin nhạy cảm, hãy xem [bài viết này](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="fdbe6-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="fdbe6-108">Nếu dùng Outlook trên web (trước đây là **OWA**): khi soạn thư email, chỉ cần bấm **bảo vệ** trong OWA.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="fdbe6-109">Quyền này sẽ áp dụng "không chuyển tiếp".</span><span class="sxs-lookup"><span data-stu-id="fdbe6-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="fdbe6-110">Bấm vào **thay đổi quyền** và chọn **mã hóa** để chỉ mã hóa thư.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="fdbe6-111">Nếu dùng **Outlook Client**: để gửi thư được mã hóa từ Outlook 2013 hoặc 2016, hoặc Outlook 2016 for Mac, hãy chọn quyền **tùy chọn**  >  **Permissions**, sau đó chọn tùy chọn bảo vệ bạn cần.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="fdbe6-112">Để **tự động mã hóa tất cả email** được gửi đến một số người nhận nhất định hoặc các tổ chức đối tác bên ngoài, bạn cần tạo một quy tắc truyền dẫn dòng thư trong Trung tâm quản trị Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdbe6-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="fdbe6-113">Hướng dẫn chi tiết được cung cấp trong [bài viết hỗ trợ này](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="fdbe6-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

