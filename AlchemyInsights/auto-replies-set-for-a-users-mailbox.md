---
title: Đặt trả lời tự động cho một hộp thư
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
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715151"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="72686-102">Đặt trả lời tự động cho hộp thư của người dùng</span><span class="sxs-lookup"><span data-stu-id="72686-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="72686-103">**Phương pháp 1**</span><span class="sxs-lookup"><span data-stu-id="72686-103">**Method 1**</span></span>

1. <span data-ttu-id="72686-104">Đăng nhập vào cổng thông tin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="72686-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="72686-105">Đi tới **người dùng > người dùng hiện hoạt** (hoặc **nhóm > hộp thư chung** nếu bạn đặt này trên hộp thư chung).</span><span class="sxs-lookup"><span data-stu-id="72686-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="72686-106">Chọn một người dùng có hộp thư Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="72686-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="72686-107">Trên menu bay ra ở bên phải, hãy đi đến **thiết đặt thư > trả lời tự động** (nếu đó là hộp thư chung, chỉ cần bấm vào **trả lời tự động** trên đường bay).</span><span class="sxs-lookup"><span data-stu-id="72686-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="72686-108">**Phương pháp 2**</span><span class="sxs-lookup"><span data-stu-id="72686-108">**Method 2**</span></span>

1. <span data-ttu-id="72686-109">Đăng nhập vào cổng thông tin quản trị Microsoft 365 bằng thông tin xác thực người quản trị.</span><span class="sxs-lookup"><span data-stu-id="72686-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="72686-110">Bung rộng **Trung tâm quản trị**, rồi bấm vào **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="72686-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="72686-111">Bấm vào ảnh ở góc trên bên phải, bấm vào **một người dùng khác**, rồi chọn hộp thư người dùng mà bạn muốn thay đổi.</span><span class="sxs-lookup"><span data-stu-id="72686-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="72686-112">Ở bên trái, chọn **tùy chọn**, bấm vào **sắp xếp email**, rồi bấm **trả lời tự động.**</span><span class="sxs-lookup"><span data-stu-id="72686-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="72686-113">**Phương pháp 3**</span><span class="sxs-lookup"><span data-stu-id="72686-113">**Method 3**</span></span>

<span data-ttu-id="72686-114">Chạy lệnh ghép ngắn sau đây trong Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="72686-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="72686-115">Các PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="72686-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="72686-116">Để biết thêm thông tin về lệnh ghép ngắn này, hãy xem mục [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="72686-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
