---
title: Bỏ qua khóa kích hoạt trên các thiết bị iOS giám sát bằng InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757322"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="e9dbf-102">Bỏ qua khóa kích hoạt trên các thiết bị iOS giám sát bằng InTune</span><span class="sxs-lookup"><span data-stu-id="e9dbf-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="e9dbf-103">Khả năng bỏ qua khóa kích hoạt trên thiết bị iOS giúp bạn phục hồi dễ dàng hơn từ tình huống mà người dùng bật khóa kích hoạt trên thiết bị công ty, rồi rời khỏi công ty.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="e9dbf-104">Các site Pre-requiđể bỏ qua khóa kích hoạt bao gồm:</span><span class="sxs-lookup"><span data-stu-id="e9dbf-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="e9dbf-105">Thiết bị là "có giám sát".</span><span class="sxs-lookup"><span data-stu-id="e9dbf-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="e9dbf-106">Khóa kích hoạt đã được kích hoạt thành công bằng cách sử dụng chính sách hạn chế thiết bị iOS trong InTune.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="e9dbf-107">Ngoài ra, khi bỏ qua khóa kích hoạt, bạn nên:</span><span class="sxs-lookup"><span data-stu-id="e9dbf-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="e9dbf-108">Thể chất có thiết bị bị xóa sổ.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="e9dbf-109">Sao chép mã trước khi bạn phát hành xóa.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="e9dbf-110">**Lưu ý:** Mã xóa không phân biệt chữ hoa/thường, vì vậy các ký tự "-" không bắt buộc.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="e9dbf-111">Để biết chi tiết, hãy xem [bỏ qua khóa kích hoạt trên các thiết bị iOS có giám sát với InTune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="e9dbf-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="e9dbf-112">**DIỄN**</span><span class="sxs-lookup"><span data-stu-id="e9dbf-112">**FAQ**</span></span>

<span data-ttu-id="e9dbf-113">Hỏi: **tôi đã ban hành một hành động từ xa để loại bỏ dữ liệu công ty khỏi thiết bị và bây giờ nó bị kẹt trong trạng thái đang chờ xử lý.**</span><span class="sxs-lookup"><span data-stu-id="e9dbf-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="e9dbf-114">A: đối với hành động từ xa để hoàn thành thành công, thiết bị đích phải trực tuyến và khỏe mạnh.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="e9dbf-115">Trong những tình huống sau đây, hành động từ xa vẫn nằm trong trạng thái đang chờ 30 ngày hoặc cho đến khi thiết bị thừa nhận lệnh khi thiết bị:</span><span class="sxs-lookup"><span data-stu-id="e9dbf-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="e9dbf-116">Không có kết nối.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-116">Does not have connectivity.</span></span>
- <span data-ttu-id="e9dbf-117">Mất trạng thái quản lý của nó bằng InTune.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="e9dbf-118">Nếu bạn cho rằng thiết bị không còn được kiểm tra và nó sẽ không loại bỏ dữ liệu công ty, hãy chọn xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="e9dbf-119">Việc xóa bỏ bản ghi thiết bị để nó không còn xuất hiện trong danh sách các thiết bị InTune.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="e9dbf-120">Đối với thiết bị hoạt động trở lại, người dùng của nó phải đăng ký lại thiết bị.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="e9dbf-121">Hỏi: **tại sao những hành động từ xa nhất định không sẵn dùng cho tôi để sử dụng?**</span><span class="sxs-lookup"><span data-stu-id="e9dbf-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="e9dbf-122">A: không phải tất cả các nền tảng hỗ trợ tất cả các hành động thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="e9dbf-123">Các hành động từ xa sau đây là nền tảng cụ thể.</span><span class="sxs-lookup"><span data-stu-id="e9dbf-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="e9dbf-124">Bỏ qua khóa kích hoạt (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="e9dbf-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="e9dbf-125">Bắt đầu mới (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="e9dbf-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="e9dbf-126">Chế độ bị mất (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="e9dbf-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="e9dbf-127">Định vị thiết bị (chỉ dành cho iOS)</span><span class="sxs-lookup"><span data-stu-id="e9dbf-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="e9dbf-128">Khởi động lại (chỉ dành cho Windows)</span><span class="sxs-lookup"><span data-stu-id="e9dbf-128">Restart (Windows only)</span></span>

<span data-ttu-id="e9dbf-129">Để biết thêm chi tiết về từng hành động, hãy xem các [hành động của thiết bị sẵn dùng](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="e9dbf-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>