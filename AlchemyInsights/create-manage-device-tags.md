---
title: Tạo và quản lý thẻ hoặc nhóm thiết bị
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731973"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="b27b7-102">Tạo và quản lý thẻ hoặc nhóm thiết bị</span><span class="sxs-lookup"><span data-stu-id="b27b7-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="b27b7-103">Thêm thẻ trên thiết bị để tạo sự liên kết nhóm lô-gic.</span><span class="sxs-lookup"><span data-stu-id="b27b7-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="b27b7-104">Thẻ thiết bị hỗ trợ ánh xạ phù hợp trên mạng, cho phép bạn đính kèm các thẻ khác nhau để chụp ngữ cảnh và cho phép tạo danh sách động như một phần của sự cố.</span><span class="sxs-lookup"><span data-stu-id="b27b7-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="b27b7-105">Thẻ có thể được sử dụng như một bộ lọc trong dạng xem danh sách Thiết bị hoặc để nhóm các thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b27b7-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="b27b7-106">Để biết thêm thông tin về tính năng nhóm thiết bị, hãy [xem Tạo và quản lý thẻ thiết bị](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="b27b7-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="b27b7-107">Bạn có thể thêm thẻ trên thiết bị bằng cách:</span><span class="sxs-lookup"><span data-stu-id="b27b7-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="b27b7-108">Sử dụng cổng thông tin</span><span class="sxs-lookup"><span data-stu-id="b27b7-108">Using the portal</span></span>

- <span data-ttu-id="b27b7-109">Đặt giá trị khóa đăng ký</span><span class="sxs-lookup"><span data-stu-id="b27b7-109">Setting a registry key value</span></span>
 
<span data-ttu-id="b27b7-110">**Lưu ý:** Có thể có độ trễ giữa thời gian thẻ được thêm vào một thiết bị và tính khả dụng của thẻ đó trong danh sách thiết bị và trang thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b27b7-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="b27b7-111">Để thêm thẻ thiết bị bằng API, hãy xem [Thêm hoặc loại bỏ thẻ thiết bị API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="b27b7-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="b27b7-112">Thêm và quản lý thẻ thiết bị bằng cổng thông tin</span><span class="sxs-lookup"><span data-stu-id="b27b7-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="b27b7-113">Chọn thiết bị mà bạn muốn quản lý thẻ trên đó.</span><span class="sxs-lookup"><span data-stu-id="b27b7-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="b27b7-114">Bạn có thể chọn hoặc tìm kiếm một thiết bị từ dạng xem bất kỳ trong các dạng xem sau:</span><span class="sxs-lookup"><span data-stu-id="b27b7-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="b27b7-115">**Bảng điều khiển hoạt động bảo mật** Chọn tên thiết bị từ phần Các thiết bị hàng đầu với cảnh báo hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="b27b7-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="b27b7-116">**Hàng đợi cảnh báo** - Chọn tên thiết bị bên cạnh biểu tượng thiết bị từ hàng đợi cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="b27b7-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="b27b7-117">**Danh sách thiết** bị - Chọn tên thiết bị từ danh sách thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b27b7-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="b27b7-118">**Hộp tìm kiếm** - Chọn Thiết bị từ menu thả xuống, rồi nhập tên thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b27b7-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="b27b7-119">Bạn cũng có thể đến trang cảnh báo thông qua dạng xem tệp và IP.</span><span class="sxs-lookup"><span data-stu-id="b27b7-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="b27b7-120">Chọn **Quản lý Thẻ** từ hàng hành động Phản hồi.</span><span class="sxs-lookup"><span data-stu-id="b27b7-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="b27b7-121">Nhập để tìm hoặc tạo thẻ.</span><span class="sxs-lookup"><span data-stu-id="b27b7-121">Type to find or create tags.</span></span>

<span data-ttu-id="b27b7-122">Thẻ được thêm vào chế độ xem thiết bị và được phản ánh trong dạng xem danh sách Thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b27b7-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="b27b7-123">Sau đó bạn có thể sử dụng bộ lọc Thẻ để xem danh sách thiết bị liên quan.</span><span class="sxs-lookup"><span data-stu-id="b27b7-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="b27b7-124">Để biết thêm thông tin, hãy [xem Tạo và quản lý thẻ thiết bị](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="b27b7-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>