---
title: Định vị mất thiết bị iOS với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: 70f12328813a312631c67cd72cc75559ed2eca1b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675214"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="d56ec-102">Định vị mất thiết bị iOS với InTune</span><span class="sxs-lookup"><span data-stu-id="d56ec-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="d56ec-103">Bật chế độ bị mất trên thiết bị iOS cho phép người quản trị có thư và liên hệ với số điện thoại được hiển thị trên màn hình khóa.</span><span class="sxs-lookup"><span data-stu-id="d56ec-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="d56ec-104">Sau khi chế độ bị mất được bật người quản trị có thể sử dụng hành động định vị thiết bị để xác định vị trí thực của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="d56ec-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="d56ec-105">Hành động định vị thiết bị trong InTune hoạt động với thiết bị iOS để hiển thị vị trí của một thiết bị cụ thể trên bản đồ.</span><span class="sxs-lookup"><span data-stu-id="d56ec-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="d56ec-106">Sử dụng hành động này yêu cầu thiết bị iOS được in:</span><span class="sxs-lookup"><span data-stu-id="d56ec-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="d56ec-107">Chế độ giám sát</span><span class="sxs-lookup"><span data-stu-id="d56ec-107">Supervised mode</span></span>
- <span data-ttu-id="d56ec-108">Chế độ bị mất</span><span class="sxs-lookup"><span data-stu-id="d56ec-108">Lost mode</span></span>

<span data-ttu-id="d56ec-109">Để biết thêm thông tin, hãy xem [bật chế độ bị mất trên thiết bị iOS/iPadOS có InTune](https://docs.microsoft.com/intune/device-lost-mode) và [xác định vị trí bị mất hoặc bị đánh cắp các thiết bị iOS/Ipados với InTune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="d56ec-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="d56ec-110">**DIỄN**</span><span class="sxs-lookup"><span data-stu-id="d56ec-110">**FAQ**</span></span>

<span data-ttu-id="d56ec-111">Hỏi: tôi đã ban hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị và bây giờ nó bị kẹt trong trạng thái đang chờ xử lý.</span><span class="sxs-lookup"><span data-stu-id="d56ec-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="d56ec-112">A: đối với hành động từ xa để hoàn thành thành công, thiết bị đích phải trực tuyến và khỏe mạnh.</span><span class="sxs-lookup"><span data-stu-id="d56ec-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="d56ec-113">Trong những tình huống sau đây, hành động từ xa vẫn nằm trong trạng thái đang chờ 30 ngày hoặc cho đến khi thiết bị thừa nhận lệnh:</span><span class="sxs-lookup"><span data-stu-id="d56ec-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="d56ec-114">Khi thiết bị không có kết nối</span><span class="sxs-lookup"><span data-stu-id="d56ec-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="d56ec-115">Khi thiết bị mất trạng thái quản lý của nó bằng InTune</span><span class="sxs-lookup"><span data-stu-id="d56ec-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="d56ec-116">Nếu bạn cho rằng thiết bị không còn được kiểm tra tại đó, và nó sẽ không thể loại bỏ dữ liệu của công ty, chọn xóa.</span><span class="sxs-lookup"><span data-stu-id="d56ec-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="d56ec-117">Việc xóa bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách các thiết bị InTune.</span><span class="sxs-lookup"><span data-stu-id="d56ec-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="d56ec-118">Nếu thiết bị trở thành hoạt động trở lại, người dùng sẽ phải đăng ký lại nó.</span><span class="sxs-lookup"><span data-stu-id="d56ec-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="d56ec-119">Hỏi: tại sao những hành động từ xa nhất định không sẵn dùng cho tôi để sử dụng?</span><span class="sxs-lookup"><span data-stu-id="d56ec-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="d56ec-120">A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="d56ec-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="d56ec-121">Các hành động từ xa sau đây là nền tảng cụ thể, do đó, chúng chỉ sẵn dùng cho những nền tảng được ghi chú.</span><span class="sxs-lookup"><span data-stu-id="d56ec-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="d56ec-122">Bỏ qua khóa kích hoạt (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="d56ec-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="d56ec-123">Bắt đầu mới (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="d56ec-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="d56ec-124">Chế độ bị mất (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="d56ec-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="d56ec-125">Định vị thiết bị (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="d56ec-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="d56ec-126">Khởi động lại (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="d56ec-126">Restart (Windows only)</span></span>

<span data-ttu-id="d56ec-127">Để biết thêm chi tiết về từng hành động, hãy xem các [hành động của thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="d56ec-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>