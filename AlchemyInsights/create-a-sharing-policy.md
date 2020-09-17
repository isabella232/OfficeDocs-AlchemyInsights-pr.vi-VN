---
title: Tạo chính sách chia sẻ để cho phép người dùng chia sẻ lịch của họ với những người bên ngoài tổ chức của bạn
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9ece122e0905d1afeb26e50fa0a5e049eee5c09d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806745"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="82171-102">Tạo chính sách chia sẻ để cho phép người dùng chia sẻ lịch của họ với những người bên ngoài tổ chức của bạn</span><span class="sxs-lookup"><span data-stu-id="82171-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="82171-103">Từ bảng điều khiển trung tâm quản trị Microsoft 365, hãy đi đến Exchange **quản trị**  >  **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="82171-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="82171-104">Đi đến **organization**  >  **chia sẻ**tổ chức.</span><span class="sxs-lookup"><span data-stu-id="82171-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="82171-105">Trong dạng xem danh sách, bên dưới **chia sẻ riêng lẻ**, bấm **mới** .</span><span class="sxs-lookup"><span data-stu-id="82171-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="82171-106">Trong **chính sách chia sẻ mới**, hãy nhập tên thân thiện cho chính sách chia sẻ trong hộp **tên chính sách** .</span><span class="sxs-lookup"><span data-stu-id="82171-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="82171-107">Bấm **Thêm**  để xác định quy tắc chia sẻ cho chính sách.</span><span class="sxs-lookup"><span data-stu-id="82171-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="82171-108">Trong **chia sẻ quy tắc**, hãy chọn một trong các tùy chọn sau đây để xác định các tên miền mà bạn muốn chia sẻ:</span><span class="sxs-lookup"><span data-stu-id="82171-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="82171-109">**Chia sẻ với tất cả các tên miền**</span><span class="sxs-lookup"><span data-stu-id="82171-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="82171-110">**Chia sẻ với một tên miền cụ thể**</span><span class="sxs-lookup"><span data-stu-id="82171-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="82171-111">Nếu bạn chọn **chia sẻ với một tên miền cụ thể**, hãy nhập tên miền mà bạn muốn chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="82171-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="82171-112">Nếu bạn cần nhập nhiều miền cho chính sách chia sẻ này, hãy lưu các thiết đặt cho tên miền đầu tiên, sau đó sửa các quy tắc chia sẻ để thêm nhiều tên miền.</span><span class="sxs-lookup"><span data-stu-id="82171-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="82171-113">Để xác định thông tin có thể được chia sẻ, hãy chọn hộp kiểm **chia sẻ thư mục lịch của bạn** , rồi chọn một trong các tùy chọn sau đây:</span><span class="sxs-lookup"><span data-stu-id="82171-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="82171-114">**Thông tin rảnh/bận trong lịch chỉ với thời gian**</span><span class="sxs-lookup"><span data-stu-id="82171-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="82171-115">**Thông tin rảnh/bận trên lịch với thời gian, chủ đề và địa điểm**</span><span class="sxs-lookup"><span data-stu-id="82171-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="82171-116">**Tất cả thông tin về lịch cuộc hẹn, bao gồm thời gian, chủ đề, địa điểm và tiêu đề**</span><span class="sxs-lookup"><span data-stu-id="82171-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="82171-117">Bấm **lưu** để đặt quy tắc cho chính sách chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="82171-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="82171-118">Nếu bạn muốn đặt chính sách chia sẻ này làm chính sách chia sẻ mặc định mới cho tất cả người dùng trong tổ chức của mình, hãy chọn hộp kiểm **tạo chính sách này để chia sẻ mặc định của tôi** .</span><span class="sxs-lookup"><span data-stu-id="82171-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="82171-119">Bấm **lưu** để tạo chính sách chia sẻ.</span><span class="sxs-lookup"><span data-stu-id="82171-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="82171-120">**Để biết đầy đủ về chủ đề này, vui lòng đọc:**</span><span class="sxs-lookup"><span data-stu-id="82171-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="82171-121">Tạo chính sách chia sẻ trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="82171-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="82171-122">Áp dụng chính sách chia sẻ cho hộp thư trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="82171-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="82171-123">Sửa đổi, tắt hoặc loại bỏ chính sách chia sẻ trong Exchange Online</span><span class="sxs-lookup"><span data-stu-id="82171-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)