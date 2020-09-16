---
title: Gửi email đến thư mục email rác
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769205"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="a8e44-102">Gửi email đến thư mục email rác</span><span class="sxs-lookup"><span data-stu-id="a8e44-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="a8e44-103">Nếu bạn thấy các thư gửi đi được đánh dấu là thư rác, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="a8e44-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="a8e44-104">Nếu bạn chưa có, hãy cân nhắc đặt [cấu hình thông báo chính sách thư rác](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="a8e44-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="a8e44-105">Sử dụng theo [dõi thư](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) để xem liệu thư gửi đi có **thư rác** giá trị sự kiện với chi tiết bổ sung: **sử dụng hồ bơi chuyển phát cao rủi ro**.</span><span class="sxs-lookup"><span data-stu-id="a8e44-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="a8e44-106">Đối với những thư này, hãy kiểm tra nội dung thư để xem những gì có thể được xem là thư rác.</span><span class="sxs-lookup"><span data-stu-id="a8e44-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="a8e44-107">Ví dụ: chữ ký đôi khi có thể gây ra sự cố đối với nhiều người dùng.</span><span class="sxs-lookup"><span data-stu-id="a8e44-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="a8e44-108">Nếu bạn có nhiều ví dụ về các thư gửi đi chính đáng được đánh dấu là thư rác, hãy mở một vé hỗ trợ và yêu cầu nhân viên hỗ trợ gửi thư là dương tính false cho các nhà phân tích thư rác của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="a8e44-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="a8e44-109">Hãy chuẩn bị để cung cấp các thư mẫu bao gồm tất cả các tiêu đề thư.</span><span class="sxs-lookup"><span data-stu-id="a8e44-109">Be prepared to provide sample messages that include all message headers.</span></span>
