---
title: Khắc phục sự cố gửi email cho thư mục công cộng kích hoạt thư
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716374"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="bf4aa-102">Khắc phục sự cố gửi email cho thư mục công cộng kích hoạt thư</span><span class="sxs-lookup"><span data-stu-id="bf4aa-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="bf4aa-103">Nếu người gửi bên ngoài không thể gửi thư đến thư mục công cộng kích hoạt thư của bạn, và các bên gửi nhận được lỗi: **không thể tìm thấy (550 5.4.1)**, kiểm tra miền email cho thư mục công cộng được cấu hình là một miền chuyển tiếp nội bộ thay vì một miền uỷ quyền:</span><span class="sxs-lookup"><span data-stu-id="bf4aa-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="bf4aa-104">Mở [Trung tâm quản trị Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="bf4aa-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="bf4aa-105">Đi tới \> **miền được chấp nhận** **dòng thư** , chọn miền chấp nhận, sau đó bấm vào **chỉnh sửa**.</span><span class="sxs-lookup"><span data-stu-id="bf4aa-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="bf4aa-106">Trong trang thuộc tính mở ra, nếu loại miền được đặt thành **uỷ**quyền, thay đổi giá trị chuyển **tiếp nội bộ** và sau đó bấm **lưu**.</span><span class="sxs-lookup"><span data-stu-id="bf4aa-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="bf4aa-107">Nếu người gửi bên ngoài nhận được lỗi **bạn không có quyền (550 5.7.13)**, hãy chạy lệnh sau trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem quyền ẩn danh trong thư mục công cộng:</span><span class="sxs-lookup"><span data-stu-id="bf4aa-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="bf4aa-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ví dụ: `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="bf4aa-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="bf4aa-109">Để cho phép người dùng bên ngoài gửi email đến thư mục công cộng này, thêm truy cập CreateItems quyền người dùng ẩn danh.</span><span class="sxs-lookup"><span data-stu-id="bf4aa-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="bf4aa-110">Ví dụ: `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="bf4aa-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
