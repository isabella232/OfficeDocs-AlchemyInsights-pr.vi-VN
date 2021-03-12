---
title: Sửa chữa chính sách đối tượng thuê (ghi đè hành động)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748983"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="06118-102">Sửa chữa chính sách đối tượng thuê (ghi đè hành động)</span><span class="sxs-lookup"><span data-stu-id="06118-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="06118-103">Chính sách chống thư rác trong đối tượng thuê của bạn bị ảnh hưởng trong thư này.</span><span class="sxs-lookup"><span data-stu-id="06118-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="06118-104">Để xem lại chính sách, hãy làm như sau:</span><span class="sxs-lookup"><span data-stu-id="06118-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="06118-105">Truy nhập [Trung tâm tuân thủ & bảo mật của Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), rồi đi tới chính sách chống thư rác về **quản lý mối đe dọa**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="06118-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="06118-106">Kiểm tra xem **nguồn chính sách** cho biết như sau:  **Thêm-XHeader/Modifysubject/Redirect/Delete/No Action/Bcc Message**</span><span class="sxs-lookup"><span data-stu-id="06118-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="06118-107">Nếu vậy, trên tab **tùy chỉnh** , hãy kiểm tra các thiết đặt của chính sách ảnh hưởng đến thư.</span><span class="sxs-lookup"><span data-stu-id="06118-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="06118-108">Có thể các **thiết đặt tiêu chuẩn** được áp dụng cho tất cả các khách hàng bảo vệ Exchange Online đã ảnh hưởng đến thư.</span><span class="sxs-lookup"><span data-stu-id="06118-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="06118-109">Để biết thêm thông tin về cách cấu hình chính sách bộ lọc thư rác, hãy xem [cấu hình chính sách bộ lọc thư rác của bạn](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="06118-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
