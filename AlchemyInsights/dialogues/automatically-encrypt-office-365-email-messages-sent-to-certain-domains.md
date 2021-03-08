---
title: Tự động mã hóa các thư email Office 365 được gửi đến một số tên miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527600"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="275dd-102">Tự động mã hóa các thư email Office 365 được gửi đến một số tên miền</span><span class="sxs-lookup"><span data-stu-id="275dd-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="275dd-103">Từ [Trung tâm quản trị Exchange](https://outlook.office365.com/ecp/), chọn **quy tắc > dòng thư**.</span><span class="sxs-lookup"><span data-stu-id="275dd-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="275dd-104">Bấm vào biểu tượng **(+) mới** , rồi bấm vào **áp dụng mã hóa thư Office 365 và bảo vệ quyền đối với thư**.</span><span class="sxs-lookup"><span data-stu-id="275dd-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="275dd-105">Trong **tên**, hãy nhập tên cho quy tắc, chẳng hạn như *mã hóa thư được gửi đến contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="275dd-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="275dd-106">Trong **áp dụng quy tắc này nếu**, chọn **miền > người nhận là**.</span><span class="sxs-lookup"><span data-stu-id="275dd-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="275dd-107">Nhập tên miền, chẳng hạn như **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="275dd-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="275dd-108">Bấm vào biểu tượng **Thêm (+)** , rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="275dd-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="275dd-109">Bên cạnh trường **thực hiện các bước sau** , hãy bấm **chọn một**.</span><span class="sxs-lookup"><span data-stu-id="275dd-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="275dd-110">Trong menu thả xuống của **mẫu RMS** , chọn **mã hóa**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="275dd-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="275dd-111">(Nếu bạn không thấy tùy chọn này, có nghĩa là gói đăng ký của bạn không bao gồm mã hóa tự động.</span><span class="sxs-lookup"><span data-stu-id="275dd-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="275dd-112">Tuy nhiên, bạn có thể thêm nó!</span><span class="sxs-lookup"><span data-stu-id="275dd-112">But you can add it!)</span></span>
9. <span data-ttu-id="275dd-113">Chọn bất kỳ lựa chọn tùy chọn nào (từ danh sách các lựa chọn tùy chọn mà bạn có thể thực hiện tại thời điểm này, nhiều phần có thể còn lại với cài đặt mặc định cho đơn giản hơn).</span><span class="sxs-lookup"><span data-stu-id="275dd-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="275dd-114">Bấm vào **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="275dd-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="275dd-115">Bạn luôn có thể quay lại và chỉnh sửa quy tắc này sau này.</span><span class="sxs-lookup"><span data-stu-id="275dd-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="275dd-116">Để biết thêm thông tin về cách tạo quy tắc cho mã hóa, hãy xem mục [xác định quy tắc dòng thư để mã hóa thư email trong Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="275dd-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>