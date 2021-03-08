---
title: Tự động di chuyển thư email đến hộp thư lưu trữ
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
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527747"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="34547-102">Tự động di chuyển thư email đến hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="34547-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="34547-103">Sau đây là cách thiết lập chính sách để tự động di chuyển email cũ của người dùng vào hộp thư lưu trữ:</span><span class="sxs-lookup"><span data-stu-id="34547-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="34547-104">Đi đến [**bảo mật &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **quản trị dữ liệu** tuân thủ  >   để xác nhận một hộp thư lưu trữ đã được kích hoạt cho người dùng.</span><span class="sxs-lookup"><span data-stu-id="34547-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="34547-105">Nếu chưa có, hãy bấm **bật** sau đó **có** trong hộp cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="34547-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="34547-106">Đi đến [**Trung tâm quản trị Exchange > quản lý tuân thủ > thẻ duy trì**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="34547-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="34547-107">Chọn biểu tượng + sau đó chọn **tự động áp dụng cho toàn bộ hộp thư**.</span><span class="sxs-lookup"><span data-stu-id="34547-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="34547-108">Gán tên cho thẻ duy trì, rồi chọn **di chuyển đến lưu trữ**.</span><span class="sxs-lookup"><span data-stu-id="34547-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="34547-109">Đối với khoảng thời gian lưu giữ, hãy nhập thời gian bạn muốn, chẳng hạn như 90 ngày.</span><span class="sxs-lookup"><span data-stu-id="34547-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="34547-110">Bấm vào **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="34547-110">Click **Save**.</span></span>
5. <span data-ttu-id="34547-111">Bây giờ, tạo chính sách duy trì: chọn **chính sách duy trì**, chọn biểu tượng để thêm chính sách mới.</span><span class="sxs-lookup"><span data-stu-id="34547-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="34547-112">Gán tên cho chính sách duy trì, rồi bấm và cuộn để tìm và thêm thẻ duy trì mà bạn vừa tạo ra.</span><span class="sxs-lookup"><span data-stu-id="34547-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="34547-113">Bấm vào **Lưu**.</span><span class="sxs-lookup"><span data-stu-id="34547-113">Click **Save**.</span></span>
7. <span data-ttu-id="34547-114">Cuối cùng, áp dụng chính sách duy trì cho hộp thư của người dùng: vẫn trong Trung tâm quản trị Exchange, đi đến  >  **hộp thư** của người nhận.</span><span class="sxs-lookup"><span data-stu-id="34547-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="34547-115">Chọn tất cả những người dùng bạn muốn áp dụng chính sách, rồi chọn **chỉnh sửa** (biểu tượng bút chì).</span><span class="sxs-lookup"><span data-stu-id="34547-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="34547-116">Trong hộp thoại, bấm vào **tính năng hộp thư**.</span><span class="sxs-lookup"><span data-stu-id="34547-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="34547-117">Bên dưới **chính sách duy trì**, áp dụng chính sách mà bạn vừa tạo > **lưu**.</span><span class="sxs-lookup"><span data-stu-id="34547-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="34547-118">Để biết hướng dẫn về cách áp dụng chính sách cho tất cả người dùng, hãy xem [áp dụng chính sách duy trì cho hộp thư](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="34547-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
