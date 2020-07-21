---
title: Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hoá
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198366"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="b0f1c-102">Người dùng nhận được lỗi AADSTS7000112 yammer bị vô hiệu hoá</span><span class="sxs-lookup"><span data-stu-id="b0f1c-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="b0f1c-103">Nếu bạn nhận được lỗi "AADSTS7000112: Application ' 00000005-0000-0ff1-ce00-000000000000 ' (yammer) bị vô hiệu hoá", sự cố tồn tại với các dịch vụ chính trong Azure quảng cáo.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="b0f1c-104">Quản trị viên có thể đã vô hiệu hoá dịch vụ chính để chặn truy cập vào yammer.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="b0f1c-105">Vô hiệu hoá dịch vụ chính không được khuyến nghị và có thể gây ra sự cố khác.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="b0f1c-106">Để biết thêm thông tin về phương pháp được hỗ trợ để chặn người dùng truy cập vào yammer, [hãy xem tắt truy cập yammer cho người dùng Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="b0f1c-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="b0f1c-107">Để khắc phục sự cố này trong cổng thông tin Azure và quyền truy cập của người dùng vào yammer:</span><span class="sxs-lookup"><span data-stu-id="b0f1c-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="b0f1c-108">Mở trang Azure Active Directory và chọn **ứng dụng doanh nghiệp** trong **quản lý** trong ngăn điều hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="b0f1c-109">Nhập **Office 365 yammer** vào hộp tìm kiếm, và chọn tên ứng dụng để mở cài đặt.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="b0f1c-110">Chọn thuộc **tính** trong **quản lý** trong ngăn điều hướng bên trái.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="b0f1c-111">Đặt giá trị **cho phép người dùng đăng nhập?** **có**, và sau đó chọn **lưu**.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="b0f1c-112">Đăng nhập lại vào yammer.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-112">Sign in to Yammer again.</span></span> <span data-ttu-id="b0f1c-113">Bạn có thể cần phải xóa cookie.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-113">You might need to clear cookies.</span></span>

<span data-ttu-id="b0f1c-114">Ngoài ra, chạy lệnh PowerShell để đặt giá trị.</span><span class="sxs-lookup"><span data-stu-id="b0f1c-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="b0f1c-115">Để biết thêm thông tin, hãy xem ["xin lỗi, nhưng chúng tôi đang gặp sự cố khi đăng nhập bạn vào" lỗi nếu bạn bấm vào ngăn xếp yammer trong Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b0f1c-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 