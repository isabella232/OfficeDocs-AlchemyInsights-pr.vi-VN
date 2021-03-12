---
title: Ngừng tin nhắn di chuyển sang tự động lưu trữ
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749815"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a><span data-ttu-id="b12d1-102">Ngừng tin nhắn di chuyển sang tự động lưu trữ</span><span class="sxs-lookup"><span data-stu-id="b12d1-102">Stop messages from moving to the archive automatically</span></span>

<span data-ttu-id="b12d1-103">Nếu bạn đang sử dụng chính sách duy trì, bạn có thể thay đổi độ tuổi lưu giữ trong chính sách đó để ngăn không cho thư tự động lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="b12d1-103">If you are using a retention policy, you can change the retention age in that policy to stop messages from archiving automatically.</span></span> <span data-ttu-id="b12d1-104">Dưới đây là cách thực hiện:</span><span class="sxs-lookup"><span data-stu-id="b12d1-104">Here's how:</span></span>

1. <span data-ttu-id="b12d1-105">Trong [Trung tâm quản trị Exchange](https://go.microsoft.com/fwlink/?linkid=2059104), chọn thẻ duy trì **quản lý tuân thủ**  >  .</span><span class="sxs-lookup"><span data-stu-id="b12d1-105">In the [Exchange admin center](https://go.microsoft.com/fwlink/?linkid=2059104), choose **compliance management** > **retention tags**.</span></span> <span data-ttu-id="b12d1-106">Xác định vị trí của bạn để di chuyển đến thẻ duy trì lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="b12d1-106">Locate your Move to Archive retention tag.</span></span>
2. <span data-ttu-id="b12d1-107">Trong thẻ duy trì, thay đổi khoảng thời gian lưu giữ (thời gian lưu trữ) để **không bao giờ** ngừng các mục được tự động lưu trữ bởi chính sách duy trì.</span><span class="sxs-lookup"><span data-stu-id="b12d1-107">In the retention tag, change the retention period (archive period) to **Never** to stop items from being automatically archived by a retention policy.</span></span>

> [!NOTE]
> <span data-ttu-id="b12d1-108">Điều này sẽ thay đổi thiết đặt lưu trữ cho tất cả các hộp thư có thẻ lưu giữ này được áp dụng cho chúng.</span><span class="sxs-lookup"><span data-stu-id="b12d1-108">This will change the archive setting for all mailboxes with this retention tag applied to them.</span></span>
