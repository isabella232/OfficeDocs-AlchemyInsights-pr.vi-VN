---
title: Lô di chuyển thư mục công cộng không hoàn thành, Hiển thị đã đồng bộ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: 33302110249b02aef87639792ebfd9cafd6638c0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47804387"
---
# <a name="public-folder-migration-batch-not-completing-shows-synced"></a><span data-ttu-id="5598a-102">Lô di chuyển thư mục công cộng không hoàn thành, Hiển thị đã đồng bộ</span><span class="sxs-lookup"><span data-stu-id="5598a-102">Public folder migration batch not completing, shows synced</span></span>

<span data-ttu-id="5598a-103">Bạn có thể đã bắt đầu hoàn thành lô di chuyển và trạng thái của lô di chuyển tiếp tục hiển thị "đã đồng bộ" trong thời gian rất dài.</span><span class="sxs-lookup"><span data-stu-id="5598a-103">You may have initiated completion of migration batch and status of the migration batch continues showing "Synced" for very long time.</span></span> <span data-ttu-id="5598a-104">Đây là hành vi dự kiến.</span><span class="sxs-lookup"><span data-stu-id="5598a-104">This is expected behavior.</span></span>

<span data-ttu-id="5598a-105">Nó phổ biến cho trạng thái của lô di chuyển vẫn tiếp tục được đồng bộ trong một vài giờ trước khi chuyển đổi để hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="5598a-105">It's common for the status of migration batch to remain on Synced for a few hours before it switches to Completing.</span></span> <span data-ttu-id="5598a-106">Để di chuyển liên quan đến một số lượng lớn các hộp thư đích, thông thường là bạn sẽ thấy trạng thái vẫn giữ nguyên trong trạng thái đồng bộ trong hơn 24 giờ, không cung cấp các yêu cầu di chuyển thư mục công cộng nằm bên dưới.</span><span class="sxs-lookup"><span data-stu-id="5598a-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the Synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="5598a-107">Vui lòng cho phép 24-48 giờ cho lô di chuyển để hoàn thành nhiệm vụ.</span><span class="sxs-lookup"><span data-stu-id="5598a-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>
