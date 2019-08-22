---
title: Sửa chữa các vấn đề phân phối email để kích hoạt thư thư mục công cộng
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525172"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="bb97e-102">Sửa chữa các vấn đề phân phối email để kích hoạt thư thư mục công cộng</span><span class="sxs-lookup"><span data-stu-id="bb97e-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="bb97e-103">Nếu người gửi bên ngoài không thể gửi thư đến thư mục công cộng của bạn kích hoạt thư, và những người gửi nhận được lỗi: **không thể được tìm thấy (550 5.4.1)**, xác minh tên miền thư điện tử cho thư mục chung được đặt cấu hình làm miền chuyển tiếp nội bộ thay vì một miền uỷ quyền:</span><span class="sxs-lookup"><span data-stu-id="bb97e-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="bb97e-104">Mở [Trung tâm quản trị Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="bb97e-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="bb97e-105">Đi đến **luồng thư** \> **tên miền được chấp nhận**, hãy chọn các tên miền được chấp nhận, và sau đó nhấp vào **chỉnh sửa**.</span><span class="sxs-lookup"><span data-stu-id="bb97e-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="bb97e-106">Trong các thuộc tính trang đó sẽ mở ra, nếu loại miền được thiết lập để **Authoritative**, thay đổi giá trị thành **chuyển tiếp nội bộ** và sau đó nhấp vào **lưu**.</span><span class="sxs-lookup"><span data-stu-id="bb97e-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="bb97e-107">Nếu người gửi bên ngoài nhận được lỗi **bạn không có quyền (550 5.7.13)**, hãy chạy lệnh sau trong [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) để xem các quyền cho người dùng vô danh trong thư mục công cộng:</span><span class="sxs-lookup"><span data-stu-id="bb97e-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="bb97e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Ví dụ, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="bb97e-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="bb97e-109">Để cho phép người dùng bên ngoài gửi email đến thư mục chung, hãy thêm truy cập CreateItems ngay cho người dùng chưa xác định người.</span><span class="sxs-lookup"><span data-stu-id="bb97e-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="bb97e-110">Ví dụ, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="bb97e-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
