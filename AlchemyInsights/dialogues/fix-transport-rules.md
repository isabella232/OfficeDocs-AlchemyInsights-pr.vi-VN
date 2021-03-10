---
title: Sửa quy tắc truyền dẫn
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695867"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="43a16-102">Sửa quy tắc truyền dẫn</span><span class="sxs-lookup"><span data-stu-id="43a16-102">Fix transport rules</span></span>

<span data-ttu-id="43a16-103">Quy tắc dòng thư tùy chỉnh ảnh hưởng đến thư này.</span><span class="sxs-lookup"><span data-stu-id="43a16-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="43a16-104">Để xem lại quy tắc chính xác, hãy thực hiện như sau:</span><span class="sxs-lookup"><span data-stu-id="43a16-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="43a16-105">Trong kết quả nộp, bên dưới **thông tin bổ sung**, hãy lưu ý **GUID** hoặc **tên chính sách**.</span><span class="sxs-lookup"><span data-stu-id="43a16-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="43a16-106">Khởi động Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="43a16-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="43a16-107">Để biết thêm thông tin, hãy xem [mở Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="43a16-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="43a16-108">Chạy lệnh này (sử dụng GUID từ trình gửi của bạn):  **Get-TransportRule-Identity "GUID" | FL \* mô tả**\*</span><span class="sxs-lookup"><span data-stu-id="43a16-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="43a16-109">Xem lại mô tả để xem các điều kiện được cấu hình ảnh hưởng đến thư.</span><span class="sxs-lookup"><span data-stu-id="43a16-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="43a16-110">Để tìm hiểu thêm, hãy xem [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span><span class="sxs-lookup"><span data-stu-id="43a16-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
