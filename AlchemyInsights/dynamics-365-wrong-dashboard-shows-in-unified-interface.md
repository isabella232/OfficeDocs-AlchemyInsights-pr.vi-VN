---
title: Dynamics 365-không hiển thị bảng điều khiển sai trong giao diện hợp nhất trong Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711297"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="2fe0f-102">Không hiển thị bảng điều khiển sai trong giao diện hợp nhất trong Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="2fe0f-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="2fe0f-103">Có một số lý do khiến bạn có thể thấy một bảng điều khiển khác với một bảng điều bạn mong đợi:</span><span class="sxs-lookup"><span data-stu-id="2fe0f-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="2fe0f-104">Người dùng đã thiết lập bảng điều khiển mặc định của người dùng</span><span class="sxs-lookup"><span data-stu-id="2fe0f-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="2fe0f-105">Thông thường, bạn có thể xác định bảng điều khiển mặc định của người dùng được đặt nếu nút **đặt làm mặc định** không hiển thị trong thanh lệnh bảng điều khiển.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="2fe0f-106">Bảng điều khiển mặc định của người dùng sẽ ghi đè lên tất cả các bảng điều khiển mặc định khác, ngay cả khi bảng điều khiển mặc định của người dùng không có trong ứng dụng hiện tại.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="2fe0f-107">Sử dụng giải pháp thay thế sau đây để bỏ đặt bảng điều khiển mặc định của họ.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="2fe0f-108">Tạo bảng điều khiển cá nhân mới.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="2fe0f-109">Đặt bảng điều khiển mới làm mặc định của người dùng.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="2fe0f-110">Xóa bảng điều khiển đó.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="2fe0f-111">Bảng điều khiển được đặt trong sơ đồ trang</span><span class="sxs-lookup"><span data-stu-id="2fe0f-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="2fe0f-112">Bạn có thể đã thiết lập một bảng điều khiển mặc định của tổ chức bằng cách chọn một bảng điều khiển và chọn ' đặt làm mặc định ' dưới ' tùy chỉnh hệ thống '.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="2fe0f-113">Nhưng bảng điều khiển được xác định trong trình thiết kế trang web sẽ được ưu tiên trên bảng điều khiển này, nếu người dùng có quyền truy nhập vào đó.</span><span class="sxs-lookup"><span data-stu-id="2fe0f-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="2fe0f-114">Để người dùng nhìn thấy bảng điều khiển bạn đã đặt làm mặc định của tổ chức, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="2fe0f-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="2fe0f-115">Đặt bảng điều khiển đó trong sơ đồ trang</span><span class="sxs-lookup"><span data-stu-id="2fe0f-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="2fe0f-116">Loại bỏ quyền truy nhập vào bảng điều khiển được xác định trong sitemap cho những người dùng đó</span><span class="sxs-lookup"><span data-stu-id="2fe0f-116">Remove access to the sitemap defined dashboard for those users</span></span>
