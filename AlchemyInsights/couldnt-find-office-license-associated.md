---
title: Khắc phục các ứng dụng Microsoft 365 không thể tìm thấy thư được liên kết với giấy phép Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816510"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="3a892-102">Khắc phục các ứng dụng Microsoft 365 "không thể tìm thấy thông báo giấy phép Office được liên kết"</span><span class="sxs-lookup"><span data-stu-id="3a892-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="3a892-103">Nếu bạn nhận được thông báo này, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="3a892-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="3a892-104">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không chặn truy nhập Internet vào các ứng dụng Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3a892-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="3a892-105">Xem [URL và dải địa chỉ IP của Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="3a892-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="3a892-106">Loại bỏ và [gán lại giấy phép Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) cho người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="3a892-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="3a892-107">Mở một ứng dụng Office và [đăng xuất khỏi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mọi tài khoản người dùng hiện có.</span><span class="sxs-lookup"><span data-stu-id="3a892-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="3a892-108">Đi đến thiết đặt Windows > **tài** khoản  >  **email & tài khoản** và loại bỏ tất cả tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="3a892-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="3a892-109">Đi đến thiết đặt Windows > **tài khoản**  >  **Access hoặc trường học** và ngắt kết nối tất cả các tài khoản công việc ngoại trừ tài khoản bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="3a892-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="3a892-110">Đặt lại trạng thái kích hoạt Office.</span><span class="sxs-lookup"><span data-stu-id="3a892-110">Reset the Office activation state.</span></span> <span data-ttu-id="3a892-111">[Tìm hiểu cách thức](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="3a892-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="3a892-112">[Đăng nhập](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="3a892-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="3a892-113">Để biết các giải pháp khắc phục sự cố bổ sung, hãy xem các [lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="3a892-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>