---
title: 126 nhận được một hộp thư không thể tìm thấy lỗi trong OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426684"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="7f229-102">Bạn nhận được một hộp thư không tìm thấy lỗi trong Outlook trên web?</span><span class="sxs-lookup"><span data-stu-id="7f229-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="7f229-103">Nếu bạn đang sử dụng Outlook trên web và bạn nhận được một **hộp thư không thể tìm thấy** được lỗi, tài khoản mà bạn đã sử dụng để kết nối với Outlook trên web không có giấy phép Exchange Online và do đó, không có hộp thư nào được liên kết với tài khoản đó.</span><span class="sxs-lookup"><span data-stu-id="7f229-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="7f229-104">Người quản trị có thể gán giấy phép cho tài khoản của bạn bằng cách làm theo các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="7f229-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="7f229-105">Mở [Trung tâm quản trị Microsoft 365](https://portal.office.com/adminportal/home#/homepage) và đi tới **người dùng hiện hoạt** bên dưới mục **người dùng** , rồi chọn người dùng đang nhìn thấy lỗi.</span><span class="sxs-lookup"><span data-stu-id="7f229-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="7f229-106">Trong trang người dùng mở ra, hãy đi đến phần **giấy phép và ứng dụng** , chọn giá trị **vị trí** thích hợp và gán giấy phép có chứa Exchange Online (bung rộng giấy phép để xem chi tiết của nó).</span><span class="sxs-lookup"><span data-stu-id="7f229-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="7f229-107">Khi bạn đã hoàn tất, hãy bấm **lưu thay đổi**.</span><span class="sxs-lookup"><span data-stu-id="7f229-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="7f229-108">Trong một số trường hợp, nếu giấy phép đã được gán cho một tài khoản người dùng, hãy loại bỏ và gán lại giấy phép sẽ giúp giải quyết sự cố này và nhận được quyền được cung cấp đúng cách trong hệ thống:</span><span class="sxs-lookup"><span data-stu-id="7f229-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="7f229-109">Kiểm tra xem liệu M365 Exchange Online của bạn (và khác, nếu bạn có bất kỳ thuê bao nào) hiện tại và chưa hết hạn.</span><span class="sxs-lookup"><span data-stu-id="7f229-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="7f229-110">Sau khi bạn đã đảm bảo rằng đăng ký của bạn đã không hết hạn và một giấy phép hợp lệ đã được gán cho tài khoản người dùng, có thể mất đến 24 giờ để được cung cấp để được cung cấp, vì vậy bạn có thể phải đợi vấn đề của bạn để giải quyết.</span><span class="sxs-lookup"><span data-stu-id="7f229-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="7f229-111">Để biết thêm thông tin, hãy xem mục [gán và quản lý giấy phép](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="7f229-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>