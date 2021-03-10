---
title: Sửa chính sách kết nối
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695893"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="dc4ed-102">Sửa chính sách kết nối</span><span class="sxs-lookup"><span data-stu-id="dc4ed-102">Fix connection policy</span></span>

<span data-ttu-id="dc4ed-103">Email được đánh dấu an toàn và được gửi đến hộp thư đến của người dùng vì địa chỉ IP của việc gửi được đánh dấu an toàn trong chính sách bộ lọc kết nối.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="dc4ed-104">Để xem lại chính sách, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="dc4ed-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="dc4ed-105">Truy nhập [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), rồi đi tới chính sách chống thư rác về **quản lý mối đe dọa**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="dc4ed-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="dc4ed-106">Trên tab **tùy chỉnh** , hãy chọn **chính sách bộ lọc kết nối**, rồi chọn **sửa chính sách**.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="dc4ed-107">Xem lại danh sách **IP cho phép** .</span><span class="sxs-lookup"><span data-stu-id="dc4ed-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="dc4ed-108">Xem **danh sách an toàn** được bật không.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="dc4ed-109">Microsoft đăng ký sang nguồn bên thứ ba của người gửi tin cậy.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="dc4ed-110">Nếu đã bật **danh sách an toàn** , những người gửi tin cậy này không bị nhầm lẫn được đánh dấu là thư rác.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="dc4ed-111">Tôi khuyên bạn nên chọn tùy chọn này, vì nó sẽ giảm số lượng dương tính false (thư tốt được phân loại là thư rác) mà bạn nhận được.</span><span class="sxs-lookup"><span data-stu-id="dc4ed-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
