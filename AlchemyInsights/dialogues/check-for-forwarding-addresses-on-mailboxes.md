---
title: Kiểm tra địa chỉ chuyển tiếp trên hộp thư
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428159"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="7ded9-102">Kiểm tra địa chỉ chuyển tiếp trên hộp thư</span><span class="sxs-lookup"><span data-stu-id="7ded9-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="7ded9-103">Đôi khi, hacker chuyển tiếp thư email cho chính mình, vì vậy, trước tiên, chúng tôi sẽ kiểm tra các địa chỉ và quy tắc chuyển tiếp trên hộp thư.</span><span class="sxs-lookup"><span data-stu-id="7ded9-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="7ded9-104">Sau đó, chúng tôi sẽ kiểm tra Nhật ký kiểm nghiệm.</span><span class="sxs-lookup"><span data-stu-id="7ded9-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="7ded9-105">Sau đây là cách kiểm tra các địa chỉ chuyển tiếp:</span><span class="sxs-lookup"><span data-stu-id="7ded9-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="7ded9-106">Chọn **người** dùng hiện  >  **hoạt**.</span><span class="sxs-lookup"><span data-stu-id="7ded9-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="7ded9-107">Chọn người dùng có tài khoản đã bị xâm phạm.</span><span class="sxs-lookup"><span data-stu-id="7ded9-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="7ded9-108">Trong bay ra xuất hiện, bung rộng **thiết đặt thư**, rồi bấm **sửa** để **chuyển tiếp email**.</span><span class="sxs-lookup"><span data-stu-id="7ded9-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="7ded9-109">Loại bỏ bất kỳ địa chỉ chuyển tiếp nào bạn không nhận ra.</span><span class="sxs-lookup"><span data-stu-id="7ded9-109">Remove any forwarding addresses you don't recognize.</span></span>