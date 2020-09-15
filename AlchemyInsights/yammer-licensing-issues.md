---
title: Các vấn đề về cấp phép yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657298"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="677f3-102">Các vấn đề về cấp phép yammer</span><span class="sxs-lookup"><span data-stu-id="677f3-102">Yammer licensing issues</span></span>

<span data-ttu-id="677f3-103">Tất cả người dùng phải có giấy phép sử dụng dịch vụ yammer Enterprise nhưng theo mặc định là yammer không yêu cầu người dùng có giấy phép truy nhập vào dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="677f3-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="677f3-104">Khi người quản trị thay đổi thiết đặt để chặn người dùng Microsoft 365 không có giấy phép yammer, người dùng không gán giấy phép yammer Enterprise không thể truy nhập vào dịch vụ yammer.</span><span class="sxs-lookup"><span data-stu-id="677f3-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="677f3-105">Để biết thêm thông tin, hãy xem [quản lý giấy phép người dùng yammer trong Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="677f3-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="677f3-106">Khi giấy phép được loại bỏ khỏi người dùng, lát xếp yammer không còn được hiển thị và các dịch vụ khác có thể sử dụng loại bỏ giấy phép để ẩn các tính năng.</span><span class="sxs-lookup"><span data-stu-id="677f3-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="677f3-107">Trong các trường hợp khác, các tính năng vẫn có thể xuất hiện nhưng yêu cầu gán giấy phép để hoạt động.</span><span class="sxs-lookup"><span data-stu-id="677f3-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="677f3-108">**Giấy phép không nhận được Cập Nhật cho người dùng**</span><span class="sxs-lookup"><span data-stu-id="677f3-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="677f3-109">Đôi khi, người dùng được gán giấy phép nhưng vẫn không thể truy nhập vào yammer.</span><span class="sxs-lookup"><span data-stu-id="677f3-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="677f3-110">Sự chậm trễ có nhiều khả năng xảy ra khi việc gán giấy phép hàng loạt đang được tiến hành.</span><span class="sxs-lookup"><span data-stu-id="677f3-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="677f3-111">Người dùng yammer có thể không được Cập Nhật theo cùng một thứ tự như giấy phép được thay đổi trong Azure AD vì hệ thống chạy asynchronously.</span><span class="sxs-lookup"><span data-stu-id="677f3-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="677f3-112">Chờ tối đa 24 giờ trước khi mở một trường hợp hỗ trợ để báo cáo các vấn đề về đồng bộ cấp phép.</span><span class="sxs-lookup"><span data-stu-id="677f3-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="677f3-113">**Gán hàng loạt giấy phép**</span><span class="sxs-lookup"><span data-stu-id="677f3-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="677f3-114">Có thể gán giấy phép thông qua Trung tâm quản trị hoặc script PowerShell.</span><span class="sxs-lookup"><span data-stu-id="677f3-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="677f3-115">Để biết thêm thông tin, hãy xem mục [gán giấy phép cho người dùng](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) và [gán giấy phép cho tài khoản người dùng với Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="677f3-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="677f3-116">Hỗ trợ của Microsoft không cung cấp trợ giúp với việc tạo script nhưng tài liệu hướng dẫn giấy phép yammer sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="677f3-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="677f3-117">Để biết thêm thông tin, hãy xem [quản lý giấy phép yammer bằng cách dùng Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="677f3-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>