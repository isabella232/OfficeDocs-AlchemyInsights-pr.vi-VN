---
title: Bật hộp thư lưu trữ
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811728"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="1f0c5-102">Bật hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="1f0c5-102">Enable an archive mailbox</span></span>

<span data-ttu-id="1f0c5-103">Nếu bạn muốn chúng tôi chạy kiểm tra tự động để đảm bảo có thể cấu hình hộp thư lưu trữ, hãy chọn nút quay lại <--ở phía trên cùng của trang này, sau đó nhập địa chỉ email của tài khoản.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="1f0c5-104">Hộp thư lưu trữ trong Microsoft 365 (còn được gọi là lưu trữ *trực tuyến* hoặc *lưu trữ tại chỗ*) cung cấp cho người dùng có dung lượng lưu trữ email bổ sung.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="1f0c5-105">Người dùng có thể di chuyển hoặc sao chép các mục vào hộp thư lưu trữ của họ và người quản trị có thể tạo chính sách lưu trữ tự động di chuyển các mục vào hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="1f0c5-106">Sau đây là cách tạo hộp thư lưu trữ:</span><span class="sxs-lookup"><span data-stu-id="1f0c5-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="1f0c5-107">Đi tới [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="1f0c5-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="1f0c5-108">Đăng nhập vào Microsoft 365 bằng tài khoản người quản trị của bạn.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="1f0c5-109">Trong ngăn bên trái của &amp; Trung tâm tuân thủ bảo mật, chọn lưu trữ **quản trị thông tin** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="1f0c5-110">Chọn người dùng có hộp thư lưu trữ mà bạn muốn bật.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="1f0c5-111">Trong ngăn chi tiết ở bên phải, hãy bấm **bật** và sau đó bấm **có** trong thông báo cảnh báo để bật hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="1f0c5-112">Bạn cũng có thể kích hoạt hàng loạt hộp thư lưu trữ bằng cách chọn nhiều người dùng (sử dụng các phím **Shift** hoặc **Ctrl** ), rồi bấm vào **bật** trong ngăn chi tiết.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="1f0c5-113">Hộp thư chung</span><span class="sxs-lookup"><span data-stu-id="1f0c5-113">Shared mailboxes</span></span>

<span data-ttu-id="1f0c5-114">Để bật lưu trữ cho hộp thư chung, giấy phép Exchange Online Plan 2 hoặc giấy phép Exchange Online gói 1 với giấy phép lưu trữ Exchange Online là bắt buộc.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="1f0c5-115">Để bật lưu trữ cho hộp thư chung:</span><span class="sxs-lookup"><span data-stu-id="1f0c5-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="1f0c5-116">Đi đến [Trung tâm quản trị Exchange](https://outlook.office365.com/ecp) và đăng nhập bằng tài khoản người quản trị của bạn.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="1f0c5-117">Đi đến **người nhận**được  >  **chia sẻ**.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="1f0c5-118">Chọn hộp thư chung.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="1f0c5-119">Trong ngăn chi tiết ở bên phải, bên dưới **lưu trữ tại chỗ**, hãy bấm **bật**, rồi bấm **có** để bật hộp thư lưu trữ.</span><span class="sxs-lookup"><span data-stu-id="1f0c5-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="1f0c5-120">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="1f0c5-120">For more information, see:</span></span>
  
- [<span data-ttu-id="1f0c5-121">Bật hộp thư lưu trữ</span><span class="sxs-lookup"><span data-stu-id="1f0c5-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="1f0c5-122">Thiết lập chính sách lưu trữ và xóa bỏ</span><span class="sxs-lookup"><span data-stu-id="1f0c5-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
