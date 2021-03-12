---
title: Tự động mã hóa các thư email nhất định từ Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749451"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="54b89-102">Tự động mã hóa các thư email nhất định từ Office 365</span><span class="sxs-lookup"><span data-stu-id="54b89-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="54b89-103">Từ [Trung tâm quản trị Exchange](https://outlook.office365.com/ecp/), chọn **quy tắc > dòng thư**.</span><span class="sxs-lookup"><span data-stu-id="54b89-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="54b89-104">Bấm vào biểu tượng **(+) mới** , rồi bấm vào **áp dụng mã hóa thư Office 365 và bảo vệ quyền đối với thư**.</span><span class="sxs-lookup"><span data-stu-id="54b89-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="54b89-105">Trong **tên**, hãy nhập tên cho quy tắc, chẳng hạn như *mã hóa tất cả thư*.</span><span class="sxs-lookup"><span data-stu-id="54b89-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="54b89-106">Trong **áp dụng quy tắc này nếu**, chọn **[áp dụng cho tất cả các thư]**.</span><span class="sxs-lookup"><span data-stu-id="54b89-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="54b89-107">Bên cạnh trường **thực hiện các bước sau** , hãy bấm **chọn một**.</span><span class="sxs-lookup"><span data-stu-id="54b89-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="54b89-108">Trong menu thả xuống của **mẫu RMS** , chọn **mã hóa**, rồi bấm **OK**.</span><span class="sxs-lookup"><span data-stu-id="54b89-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="54b89-109">(Nếu bạn không thấy tùy chọn này, có nghĩa là gói đăng ký của bạn không bao gồm mã hóa tự động.</span><span class="sxs-lookup"><span data-stu-id="54b89-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="54b89-110">Tuy nhiên, bạn có thể thêm nó!</span><span class="sxs-lookup"><span data-stu-id="54b89-110">But you can add it!)</span></span>
7. <span data-ttu-id="54b89-111">Kiểm tra hộp kiểm **kiểm tra quy tắc này với mức độ nghiêm trọng** , rồi chọn cấp độ mong muốn.</span><span class="sxs-lookup"><span data-stu-id="54b89-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="54b89-112">Nếu công ty của bạn có nghĩa vụ hợp đồng để gửi tất cả các email đã mã hóa, tôi khuyên bạn nên đặt mức độ **cao**.</span><span class="sxs-lookup"><span data-stu-id="54b89-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="54b89-113">Bên dưới **chọn một mô hình cho quy tắc này**, hãy bấm vào thực **thi**.</span><span class="sxs-lookup"><span data-stu-id="54b89-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="54b89-114">Chọn bất kỳ lựa chọn tùy chọn nào (từ danh sách các lựa chọn tùy chọn mà bạn có thể thực hiện tại thời điểm này, nhiều phần có thể còn lại với cài đặt mặc định cho đơn giản hơn).</span><span class="sxs-lookup"><span data-stu-id="54b89-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="54b89-115">Bấm vào **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="54b89-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="54b89-116">Bạn luôn có thể quay lại và chỉnh sửa quy tắc này sau này.</span><span class="sxs-lookup"><span data-stu-id="54b89-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="54b89-117">Để biết thêm thông tin về cách tạo quy tắc cho mã hóa, hãy xem mục [xác định quy tắc dòng thư để mã hóa thư email trong Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="54b89-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

