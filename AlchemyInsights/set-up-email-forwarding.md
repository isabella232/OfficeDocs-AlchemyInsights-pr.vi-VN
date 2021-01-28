---
title: Thiết lập chuyển tiếp email
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: 4ec122967a93f707478e05ac7874cbc884a88c84
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037207"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="4f83e-102">Kiểm tra thiết đặt chuyển tiếp email cho một hộp thư</span><span class="sxs-lookup"><span data-stu-id="4f83e-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="4f83e-103">Trước hết, chuyển tiếp email phải được bật ở mức đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="4f83e-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="4f83e-104">Nếu bạn đã thiết lập chuyển tiếp email trên một hộp thư nhưng không hoạt động (bạn nhận được lỗi **"550 5.7.520 Access bị từ chối, tổ chức của bạn không cho phép chuyển tiếp bên ngoài"**), vui lòng xem [điều khiển chuyển tiếp email bên ngoài tự động trong Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4f83e-104">If you have set up email forwarding on a mailbox, but it is not working (you get an error **"550 5.7.520 Access denied, Your organization does not allow external forwarding"**) please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="4f83e-105">Thật dễ dàng để xác minh cài đặt chuyển tiếp email trên hộp thư!</span><span class="sxs-lookup"><span data-stu-id="4f83e-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="4f83e-106">Chỉ cần làm theo các bước sau.</span><span class="sxs-lookup"><span data-stu-id="4f83e-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="4f83e-107">Nếu đây là hộp thư người dùng, hãy **đi đến người dùng hiện** \> **hoạt** và chọn người dùng có hộp thư mà bạn đang chuyển tiếp.</span><span class="sxs-lookup"><span data-stu-id="4f83e-107">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding.</span></span> <span data-ttu-id="4f83e-108">Trên tab **thư** , chọn **quản lý chuyển tiếp email**.</span><span class="sxs-lookup"><span data-stu-id="4f83e-108">On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="4f83e-109">Nếu đây là hộp thư chung, hãy đi  đến \> **hộp thư nhóm được chia sẻ** và chọn hộp thư chung mà bạn đang chuyển tiếp.</span><span class="sxs-lookup"><span data-stu-id="4f83e-109">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding.</span></span> <span data-ttu-id="4f83e-110">Chọn **chỉnh sửa** để chuyển tiếp email.</span><span class="sxs-lookup"><span data-stu-id="4f83e-110">Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="4f83e-111">Để biết thêm thông tin, hãy xem [đặt cấu hình chuyển tiếp email trong Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="4f83e-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="4f83e-112">Để gửi hướng dẫn cho người dùng của bạn để họ có thể thiết lập chuyển tiếp email trên hộp thư của chính họ, hãy trỏ họ đến [chuyển tiếp email từ Microsoft 365 sang một tài khoản email khác](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span><span class="sxs-lookup"><span data-stu-id="4f83e-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="4f83e-113">Xin lưu ý rằng bạn có thể chuyển tiếp đến một địa chỉ email.</span><span class="sxs-lookup"><span data-stu-id="4f83e-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="4f83e-114">Nếu bạn cần thiết lập chuyển tiếp sang một nhóm người, hãy tạo danh sách phân phối (bên dưới **nhóm**), thêm người dùng của bạn vào đó, rồi cấu hình chuyển tiếp đến nhóm đó.</span><span class="sxs-lookup"><span data-stu-id="4f83e-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="4f83e-115">Bạn có nhân viên rời khỏi không?</span><span class="sxs-lookup"><span data-stu-id="4f83e-115">Do you have an employee leaving?</span></span> <span data-ttu-id="4f83e-116">Xem mục [loại bỏ nhân viên cũ khỏi Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) cho các bước được đề xuất.</span><span class="sxs-lookup"><span data-stu-id="4f83e-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>