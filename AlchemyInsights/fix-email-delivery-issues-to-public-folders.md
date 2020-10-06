---
title: Khắc phục sự cố chuyển phát email thành các thư mục công cộng cho phép thư
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366486"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="c27f8-102">Khắc phục sự cố chuyển phát email thành các thư mục công cộng cho phép thư</span><span class="sxs-lookup"><span data-stu-id="c27f8-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="c27f8-103">Nếu người gửi bên ngoài không thể gửi thư vào các thư mục công cộng cho phép thư của bạn và người gửi nhận được lỗi: **không thể tìm thấy (550 5.4.1)**, hãy xác nhận tên miền email cho thư mục công cộng được đặt cấu hình là tên miền chuyển tiếp nội bộ thay vì miền có thẩm quyền:</span><span class="sxs-lookup"><span data-stu-id="c27f8-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="c27f8-104">Mở [Trung tâm quản trị Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="c27f8-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="c27f8-105">Đi tới **Mail flow** \> **tên miền được chấp nhận**của dòng thư, chọn miền được chấp nhận, rồi bấm **sửa**.</span><span class="sxs-lookup"><span data-stu-id="c27f8-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="c27f8-106">Trong trang thuộc tính mở ra, nếu loại tên miền được đặt là có **thẩm quyền**, hãy thay đổi giá trị thành chuyển **tiếp nội bộ** , rồi bấm **lưu**.</span><span class="sxs-lookup"><span data-stu-id="c27f8-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="c27f8-107">Nếu người gửi bên ngoài nhận được lỗi **mà bạn không có quyền (550 5.7.13)**, hãy chạy lệnh sau đây trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem quyền đối với người dùng ẩn danh trong thư mục công cộng:</span><span class="sxs-lookup"><span data-stu-id="c27f8-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="c27f8-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Ví dụ, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="c27f8-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="c27f8-109">Để cho phép người dùng bên ngoài gửi email đến thư mục công cộng này, hãy thêm truy nhập CreateItems sang phải với người dùng ẩn danh.</span><span class="sxs-lookup"><span data-stu-id="c27f8-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="c27f8-110">Ví dụ, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="c27f8-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
