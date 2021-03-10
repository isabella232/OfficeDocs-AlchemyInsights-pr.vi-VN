---
title: Sửa chữa chính sách/thiết đặt hộp thư của người dùng
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695896"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="ecbf6-102">Sửa chữa chính sách/thiết đặt hộp thư của người dùng</span><span class="sxs-lookup"><span data-stu-id="ecbf6-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="ecbf6-103">Thiết đặt thư rác trên hộp thư ảnh hưởng đến thư này.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="ecbf6-104">Để xem lại các cài đặt, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="ecbf6-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="ecbf6-105">Khởi động Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="ecbf6-106">Để biết thêm thông tin, hãy xem [mở Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="ecbf6-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="ecbf6-107">Chạy lệnh này (sử dụng địa chỉ email của người dùng):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="ecbf6-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="ecbf6-108">Kiểm tra xem địa chỉ email của người gửi là một phần trong **Trustedsendersanddomains** hay **Blockenhsendersanddomains**.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="ecbf6-109">Nếu địa chỉ email nằm trong một trong các danh sách, bạn có thể phải loại bỏ nó.</span><span class="sxs-lookup"><span data-stu-id="ecbf6-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="ecbf6-110">Để tìm hiểu thêm, hãy xem [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="ecbf6-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
