---
title: Đặt trả lời tự động cho hộp thư
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788904"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="1532d-102">Đặt trả lời tự động cho hộp thư của người dùng</span><span class="sxs-lookup"><span data-stu-id="1532d-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="1532d-103">**Phương pháp 1**</span><span class="sxs-lookup"><span data-stu-id="1532d-103">**Method 1**</span></span>

1. <span data-ttu-id="1532d-104">Đăng nhập vào cổng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1532d-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="1532d-105">Truy cập **người dùng > người dùng đang hoạt động** (hoặc **nhóm > hộp thư dùng chung** nếu bạn đặt điều này vào hộp thư dùng chung).</span><span class="sxs-lookup"><span data-stu-id="1532d-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="1532d-106">Chọn một người dùng có hộp thư Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="1532d-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="1532d-107">Trên menu Fly-out ở bên phải, đi tới **cài đặt Mail > trả lời tự động** (nếu đó là hộp thư dùng chung, chỉ cần nhấp vào **trả lời tự động** trên Fly-out).</span><span class="sxs-lookup"><span data-stu-id="1532d-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="1532d-108">**Phương pháp 2**</span><span class="sxs-lookup"><span data-stu-id="1532d-108">**Method 2**</span></span>

1. <span data-ttu-id="1532d-109">Đăng nhập vào cổng quản trị Microsoft 365 bằng cách sử dụng uỷ nhiệm quản trị viên.</span><span class="sxs-lookup"><span data-stu-id="1532d-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="1532d-110">Mở rộng **Trung tâm quản trị**, và sau đó bấm **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1532d-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="1532d-111">Bấm vào hình ảnh ở góc trên bên phải, bấm **người dùng khác**, và sau đó chọn hộp thư người dùng mà bạn muốn thay đổi.</span><span class="sxs-lookup"><span data-stu-id="1532d-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="1532d-112">Ở bên trái, chọn **tuỳ chọn**, bấm **tổ chức E-mail**, và sau đó nhấp vào **trả lời tự động.**</span><span class="sxs-lookup"><span data-stu-id="1532d-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="1532d-113">**Phương pháp 3**</span><span class="sxs-lookup"><span data-stu-id="1532d-113">**Method 3**</span></span>

<span data-ttu-id="1532d-114">Chạy lệnh sau trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1532d-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="1532d-115">Máy PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="1532d-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="1532d-116">Để biết thêm thông tin về lệnh này, xem [thiết lập MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="1532d-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
