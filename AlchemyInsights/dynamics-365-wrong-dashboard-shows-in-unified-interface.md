---
title: Dynamics 365 - bảng điều khiển sai cho thấy trong giao diện thống nhất Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36528573"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="98ffb-102">Bảng điều khiển sai cho thấy trong giao diện thống nhất Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="98ffb-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="98ffb-103">Có rất nhiều lý do tại sao bạn có thể thấy một bảng điều khiển khác nhau hơn bạn mong đợi:</span><span class="sxs-lookup"><span data-stu-id="98ffb-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="98ffb-104">Người dùng đã thiết lập một bảng điều khiển người dùng mặc định</span><span class="sxs-lookup"><span data-stu-id="98ffb-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="98ffb-105">Thông thường bạn có thể xác định một người sử dụng bảng điều khiển mặc định được thiết lập nếu nút **Đặt làm mặc định** không hiển thị trong bảng điều khiển lệnh thanh.</span><span class="sxs-lookup"><span data-stu-id="98ffb-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="98ffb-106">Người dùng mặc định bảng sẽ ghi đè lên tất cả các mặc định trang tổng quan, thậm chí nếu người dùng mặc định bảng điều khiển không phải là các ứng dụng hiện tại.</span><span class="sxs-lookup"><span data-stu-id="98ffb-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="98ffb-107">Sử dụng các workaround sau đây để bỏ đặt của bảng điều khiển mặc định.</span><span class="sxs-lookup"><span data-stu-id="98ffb-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="98ffb-108">Tạo ra một bảng điều khiển cá nhân mới.</span><span class="sxs-lookup"><span data-stu-id="98ffb-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="98ffb-109">Đặt rằng bảng điều khiển mới như mặc định của người dùng.</span><span class="sxs-lookup"><span data-stu-id="98ffb-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="98ffb-110">Xóa bảng đó.</span><span class="sxs-lookup"><span data-stu-id="98ffb-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="98ffb-111">Bảng điều khiển được đặt trong sơ đồ trang web</span><span class="sxs-lookup"><span data-stu-id="98ffb-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="98ffb-112">Bạn có thể đã thiết lập một tổ chức mặc định bảng bằng cách chọn một bảng điều khiển và chọn 'Thiết lập như mặc định' dưới 'Tùy chỉnh các hệ thống'.</span><span class="sxs-lookup"><span data-stu-id="98ffb-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="98ffb-113">Nhưng bảng điều khiển được định nghĩa trong các thiết kế sơ đồ trang web sẽ được ưu tiên qua bảng điều khiển này, nếu người dùng có quyền truy cập vào nó.</span><span class="sxs-lookup"><span data-stu-id="98ffb-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="98ffb-114">Để người dùng xem các bảng điều khiển bạn đã thiết lập mặc định của tổ chức, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="98ffb-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="98ffb-115">Đặt rằng bảng điều khiển trong sơ đồ trang web</span><span class="sxs-lookup"><span data-stu-id="98ffb-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="98ffb-116">Loại bỏ quyền truy cập vào bảng sơ đồ trang web xác định cho những người dùng</span><span class="sxs-lookup"><span data-stu-id="98ffb-116">Remove access to the sitemap defined dashboard for those users</span></span>
