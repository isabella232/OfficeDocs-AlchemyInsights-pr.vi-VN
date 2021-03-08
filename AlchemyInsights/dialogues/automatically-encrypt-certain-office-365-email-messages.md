---
title: Tự động mã hóa một số thông điệp email trong Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527616"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="0eb40-102">Tự động mã hóa một số thông điệp email trong Office 365</span><span class="sxs-lookup"><span data-stu-id="0eb40-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="0eb40-103">Bạn có thể tự động mã hóa thư mà người dùng gửi đến một số người hoặc tổ chức bên ngoài nhất định.</span><span class="sxs-lookup"><span data-stu-id="0eb40-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="0eb40-104">Để thực hiện điều này, hãy làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="0eb40-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="0eb40-105">Từ [Trung tâm quản trị Exchange](https://outlook.office365.com/ecp/), chọn **quy tắc > dòng thư**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="0eb40-106">Bấm vào biểu tượng **(+) mới** , rồi bấm vào **áp dụng mã hóa thư Office 365 và bảo vệ quyền đối với thư**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="0eb40-107">Trong **tên**, hãy nhập tên cho quy tắc, chẳng hạn như *mã hóa thư được gửi đến DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="0eb40-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="0eb40-108">Trong **áp dụng quy tắc này nếu**, chọn **> người nhận là người này**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="0eb40-109">Trong cửa sổ **chọn thành viên** , hãy chọn tên của người mà bạn muốn áp dụng quy tắc mã hóa, rồi bấm **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="0eb40-110">Khi bạn đã hoàn tất việc thêm người dùng, hãy bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="0eb40-111">Bên cạnh trường **thực hiện các bước sau** , hãy bấm **chọn một**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="0eb40-112">Trong menu thả xuống của **mẫu RMS** , chọn **mã hóa**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="0eb40-113">(Nếu bạn không thấy tùy chọn này, có nghĩa là gói đăng ký của bạn không bao gồm mã hóa tự động.</span><span class="sxs-lookup"><span data-stu-id="0eb40-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="0eb40-114">Tuy nhiên, bạn có thể thêm nó!</span><span class="sxs-lookup"><span data-stu-id="0eb40-114">But you can add it!)</span></span>
9. <span data-ttu-id="0eb40-115">Chọn bất kỳ lựa chọn tùy chọn nào (từ danh sách các lựa chọn tùy chọn mà bạn có thể thực hiện tại thời điểm này, nhiều phần có thể còn lại với cài đặt mặc định cho đơn giản hơn).</span><span class="sxs-lookup"><span data-stu-id="0eb40-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="0eb40-116">Bấm vào **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="0eb40-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0eb40-117">Bạn luôn có thể quay lại và chỉnh sửa quy tắc này sau này.</span><span class="sxs-lookup"><span data-stu-id="0eb40-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="0eb40-118">Để biết thêm thông tin về cách tạo quy tắc cho mã hóa, hãy xem mục [xác định quy tắc dòng thư để mã hóa thư email trong Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="0eb40-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

