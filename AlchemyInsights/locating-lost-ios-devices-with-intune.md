---
title: Định vị các thiết bị iOS bị mất với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440434"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="38073-102">Định vị các thiết bị iOS bị mất với InTune</span><span class="sxs-lookup"><span data-stu-id="38073-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="38073-103">Cho phép chế độ mất trên thiết bị iOS cho phép quản trị viên có thư và số điện thoại liên hệ được hiển thị trên màn hình khóa.</span><span class="sxs-lookup"><span data-stu-id="38073-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="38073-104">Sau khi chế độ bị mất được kích hoạt quản trị viên có thể sử dụng định vị hành động thiết bị để xác định vị trí vật lý của thiết bị.</span><span class="sxs-lookup"><span data-stu-id="38073-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="38073-105">Hành động xác định thiết bị trong InTune hoạt động với thiết bị iOS để hiển thị vị trí của một thiết bị cụ thể trên bản đồ.</span><span class="sxs-lookup"><span data-stu-id="38073-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="38073-106">Sử dụng hành động này yêu cầu thiết bị iOS được trong:</span><span class="sxs-lookup"><span data-stu-id="38073-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="38073-107">Chế độ giám sát</span><span class="sxs-lookup"><span data-stu-id="38073-107">Supervised mode</span></span>
- <span data-ttu-id="38073-108">Chế độ mất</span><span class="sxs-lookup"><span data-stu-id="38073-108">Lost mode</span></span>

<span data-ttu-id="38073-109">Để biết thêm thông tin, hãy xem [bật chế độ mất trên các thiết bị iOS/iPadOS với InTune](https://docs.microsoft.com/intune/device-lost-mode) và [định vị các thiết bị bị mất hoặc đánh cắp iOS/ipados với InTune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="38073-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="38073-110">**Faq**</span><span class="sxs-lookup"><span data-stu-id="38073-110">**FAQ**</span></span>

<span data-ttu-id="38073-111">Câu hỏi: tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu của công ty khỏi thiết bị và bây giờ nó được dán ở trạng thái chờ.</span><span class="sxs-lookup"><span data-stu-id="38073-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="38073-112">A: đối với một hành động từ xa để hoàn thành thành công, các thiết bị mục tiêu phải trực tuyến và khỏe mạnh.</span><span class="sxs-lookup"><span data-stu-id="38073-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="38073-113">Trong các trường hợp sau, hành động từ xa ở trạng thái chờ trong 30 ngày, hoặc cho đến khi thiết bị thừa công lệnh:</span><span class="sxs-lookup"><span data-stu-id="38073-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="38073-114">Khi thiết bị không có kết nối</span><span class="sxs-lookup"><span data-stu-id="38073-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="38073-115">Khi thiết bị mất trạng thái quản lý với InTune</span><span class="sxs-lookup"><span data-stu-id="38073-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="38073-116">Nếu bạn cho rằng thiết bị không còn được kiểm tra và không thể xóa dữ liệu công ty, hãy chọn xóa.</span><span class="sxs-lookup"><span data-stu-id="38073-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="38073-117">Xóa loại bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách thiết bị InTune.</span><span class="sxs-lookup"><span data-stu-id="38073-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="38073-118">Nếu thiết bị trở nên hoạt động trở lại, người dùng của nó sẽ phải đăng ký lại nó.</span><span class="sxs-lookup"><span data-stu-id="38073-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="38073-119">Hỏi: tại sao một số hành động từ xa không có sẵn cho tôi để sử dụng?</span><span class="sxs-lookup"><span data-stu-id="38073-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="38073-120">A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="38073-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="38073-121">Các hành động từ xa sau đây là nền tảng cụ thể, vì vậy chúng chỉ có sẵn cho các nền tảng được ghi nhận.</span><span class="sxs-lookup"><span data-stu-id="38073-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="38073-122">Khóa kích hoạt bỏ qua (chỉ iOS)</span><span class="sxs-lookup"><span data-stu-id="38073-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="38073-123">Khởi động mới (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="38073-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="38073-124">Chế độ mất (chỉ iOS)</span><span class="sxs-lookup"><span data-stu-id="38073-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="38073-125">Xác định vị trí thiết bị (iOS chỉ)</span><span class="sxs-lookup"><span data-stu-id="38073-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="38073-126">Khởi động lại (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="38073-126">Restart (Windows only)</span></span>

<span data-ttu-id="38073-127">Để biết thêm chi tiết về từng hành động, xem [hành động của thiết bị có sẵn](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="38073-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>