---
title: Bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424285"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="1907b-102">Bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune</span><span class="sxs-lookup"><span data-stu-id="1907b-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="1907b-103">Khả năng bỏ qua khóa kích hoạt trên các thiết bị iOS giúp dễ dàng khôi phục từ tình huống mà người dùng cho phép khóa kích hoạt trên thiết bị công ty và sau đó rời khỏi công ty.</span><span class="sxs-lookup"><span data-stu-id="1907b-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="1907b-104">Pre-requisites để bỏ qua một khóa kích hoạt bao gồm:</span><span class="sxs-lookup"><span data-stu-id="1907b-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="1907b-105">Một thiết bị là "được giám sát."</span><span class="sxs-lookup"><span data-stu-id="1907b-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="1907b-106">Khóa kích hoạt được kích hoạt thành công bằng cách sử dụng chính sách hạn chế thiết bị iOS trong InTune.</span><span class="sxs-lookup"><span data-stu-id="1907b-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="1907b-107">Ngoài ra, khi bỏ qua một khóa kích hoạt, bạn nên:</span><span class="sxs-lookup"><span data-stu-id="1907b-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="1907b-108">Thể chất có thiết bị bị xóa.</span><span class="sxs-lookup"><span data-stu-id="1907b-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="1907b-109">Sao chép mã trước khi bạn phát hành xoá.</span><span class="sxs-lookup"><span data-stu-id="1907b-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="1907b-110">**Lưu ý:** Xoá mã không phải là trường hợp nhạy cảm, do đó, các ký tự "-" là không cần thiết.</span><span class="sxs-lookup"><span data-stu-id="1907b-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="1907b-111">Để biết chi tiết, xem [bỏ qua kích hoạt khóa trên các thiết bị iOS giám sát với InTune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="1907b-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="1907b-112">**Faq**</span><span class="sxs-lookup"><span data-stu-id="1907b-112">**FAQ**</span></span>

<span data-ttu-id="1907b-113">Câu hỏi: **tôi đã phát hành một hành động từ xa để loại bỏ dữ liệu của công ty khỏi thiết bị và bây giờ nó được dán ở trạng thái chờ.**</span><span class="sxs-lookup"><span data-stu-id="1907b-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="1907b-114">A: đối với một hành động từ xa để hoàn thành thành công, các thiết bị mục tiêu phải trực tuyến và khỏe mạnh.</span><span class="sxs-lookup"><span data-stu-id="1907b-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="1907b-115">Trong các trường hợp sau, hành động từ xa ở trạng thái chờ trong 30 ngày, hoặc cho đến khi thiết bị thừa công lệnh khi thiết bị:</span><span class="sxs-lookup"><span data-stu-id="1907b-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="1907b-116">Không có kết nối.</span><span class="sxs-lookup"><span data-stu-id="1907b-116">Does not have connectivity.</span></span>
- <span data-ttu-id="1907b-117">Mất trạng thái quản lý của mình với InTune.</span><span class="sxs-lookup"><span data-stu-id="1907b-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="1907b-118">Nếu bạn cho rằng một thiết bị không còn kiểm tra và nó sẽ không xóa dữ liệu công ty, hãy chọn xóa.</span><span class="sxs-lookup"><span data-stu-id="1907b-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="1907b-119">Xóa loại bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách thiết bị InTune.</span><span class="sxs-lookup"><span data-stu-id="1907b-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="1907b-120">Để thiết bị hoạt động trở lại, người dùng phải đăng ký lại thiết bị.</span><span class="sxs-lookup"><span data-stu-id="1907b-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="1907b-121">Hỏi: **tại sao một số hành động từ xa không có sẵn cho tôi để sử dụng?**</span><span class="sxs-lookup"><span data-stu-id="1907b-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="1907b-122">A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="1907b-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="1907b-123">Các hành động từ xa sau đây là nền tảng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="1907b-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="1907b-124">Khóa kích hoạt bỏ qua (chỉ iOS)</span><span class="sxs-lookup"><span data-stu-id="1907b-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="1907b-125">Khởi động mới (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="1907b-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="1907b-126">Chế độ mất (chỉ iOS)</span><span class="sxs-lookup"><span data-stu-id="1907b-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="1907b-127">Xác định vị trí thiết bị (iOS chỉ)</span><span class="sxs-lookup"><span data-stu-id="1907b-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="1907b-128">Khởi động lại (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="1907b-128">Restart (Windows only)</span></span>

<span data-ttu-id="1907b-129">Để biết thêm chi tiết về từng hành động, xem [hành động của thiết bị có sẵn](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="1907b-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>