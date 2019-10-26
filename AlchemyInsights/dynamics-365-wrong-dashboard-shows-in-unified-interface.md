---
title: Dynamics 365-bảng điều khiển hiển thị sai trong Dynamics 365 giao diện hợp nhất
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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528573"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="dc6e6-102">Bảng điều khiển không đúng Hiển thị trong Dynamics 365 giao diện hợp nhất</span><span class="sxs-lookup"><span data-stu-id="dc6e6-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="dc6e6-103">Có một số lý do khiến bạn có thể thấy một bảng thông tin khác với trang bạn mong muốn:</span><span class="sxs-lookup"><span data-stu-id="dc6e6-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="dc6e6-104">Người dùng đã đặt bảng điều khiển mặc định của người dùng</span><span class="sxs-lookup"><span data-stu-id="dc6e6-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="dc6e6-105">Thông thường, bạn có thể xác định một bảng điều khiển mặc định người dùng được thiết lập nếu nút **đặt làm mặc định** không hiển thị trong thanh lệnh bảng điều khiển.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="dc6e6-106">Bảng điều khiển mặc định người dùng sẽ ghi đè tất cả các bảng thông tin mặc định khác, ngay cả khi bảng điều khiển mặc định của người dùng không có trong ứng dụng hiện tại.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="dc6e6-107">Sử dụng giải pháp sau để unset bảng điều khiển mặc định của họ.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="dc6e6-108">Tạo bảng thông tin cá nhân mới.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="dc6e6-109">Đặt bảng thông tin mới là mặc định của người dùng.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="dc6e6-110">Xóa bảng thông tin đó.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="dc6e6-111">Bảng điều khiển được đặt trong sơ đồ trang web</span><span class="sxs-lookup"><span data-stu-id="dc6e6-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="dc6e6-112">Bạn có thể đã đặt một bảng điều khiển mặc định của tổ chức bằng cách chọn một bảng thông tin và chọn ' đặt làm mặc định ' trong ' tùy chỉnh hệ thống '.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="dc6e6-113">Tuy nhiên, bảng điều khiển được xác định trong thiết kế sơ đồ trang web sẽ được ưu tiên hơn bảng điều khiển này, nếu người dùng có quyền truy cập vào nó.</span><span class="sxs-lookup"><span data-stu-id="dc6e6-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="dc6e6-114">Để có người dùng xem bảng thông tin bạn đã đặt làm mặc định của tổ chức, bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="dc6e6-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="dc6e6-115">Đặt bảng thông tin đó trong sơ đồ trang web</span><span class="sxs-lookup"><span data-stu-id="dc6e6-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="dc6e6-116">Xóa quyền truy cập vào bảng điều khiển được xác định bởi Sơ đồ trang web cho những người dùng đó</span><span class="sxs-lookup"><span data-stu-id="dc6e6-116">Remove access to the sitemap defined dashboard for those users</span></span>
