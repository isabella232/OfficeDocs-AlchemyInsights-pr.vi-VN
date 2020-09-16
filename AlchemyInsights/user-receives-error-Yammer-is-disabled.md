---
title: Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hóa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: 3a3a1b531f3d775f7e5150ce86733a3012df8d0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47796670"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="b0882-102">Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hóa</span><span class="sxs-lookup"><span data-stu-id="b0882-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="b0882-103">Nếu bạn nhận được lỗi "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (yammer) bị vô hiệu hóa", vấn đề này tồn tại với hiệu trưởng dịch vụ trong Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b0882-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="b0882-104">Người quản trị có thể đã vô hiệu hóa hiệu trưởng dịch vụ để chặn quyền truy nhập vào yammer.</span><span class="sxs-lookup"><span data-stu-id="b0882-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="b0882-105">Vô hiệu hóa hiệu trưởng của dịch vụ không được đề xuất và có thể gây ra sự cố bổ sung.</span><span class="sxs-lookup"><span data-stu-id="b0882-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="b0882-106">Để biết thêm thông tin về cách tiếp cận được hỗ trợ để chặn quyền truy nhập của người dùng vào yammer, hãy xem mục tắt [truy nhập yammer dành cho người dùng Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="b0882-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="b0882-107">Để sửa vấn đề này trong cổng thông tin Azure và khôi phục quyền truy nhập của người dùng vào yammer:</span><span class="sxs-lookup"><span data-stu-id="b0882-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="b0882-108">Mở trang Azure Active Directory, rồi chọn các **ứng dụng doanh nghiệp** bên dưới **quản lý** trong ngăn dẫn hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="b0882-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="b0882-109">Nhập **Office 365 yammer** trong hộp tìm kiếm, rồi chọn tên ứng dụng để mở thiết đặt.</span><span class="sxs-lookup"><span data-stu-id="b0882-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="b0882-110">Chọn **thuộc tính** bên dưới **quản lý** trong ngăn dẫn hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="b0882-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="b0882-111">Đặt giá trị được **kích hoạt cho người dùng đăng nhập?** để **có**, rồi chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="b0882-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="b0882-112">Đăng nhập lại vào yammer.</span><span class="sxs-lookup"><span data-stu-id="b0882-112">Sign in to Yammer again.</span></span> <span data-ttu-id="b0882-113">Bạn có thể cần xóa các cookie.</span><span class="sxs-lookup"><span data-stu-id="b0882-113">You might need to clear cookies.</span></span>

<span data-ttu-id="b0882-114">Ngoài ra, hãy chạy lệnh PowerShell để đặt giá trị.</span><span class="sxs-lookup"><span data-stu-id="b0882-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="b0882-115">Để biết thêm thông tin, hãy xem mục ["rất tiếc nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn trong" lỗi khi bạn bấm vào lát xếp yammer trong Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b0882-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 