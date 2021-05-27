---
title: Trạng thái cảm biến kiểm tra điểm cuối của Bộ bảo vệ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676542"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="b9355-102">Trạng thái cảm biến kiểm tra điểm cuối của Bộ bảo vệ</span><span class="sxs-lookup"><span data-stu-id="b9355-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="b9355-103">Lát **xếp Thiết bị có sự cố cảm** biến nằm trên bảng điều khiển Hoạt động Bảo mật.</span><span class="sxs-lookup"><span data-stu-id="b9355-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="b9355-104">Ô xếp này cung cấp thông tin về khả năng cung cấp dữ liệu cảm biến và liên lạc với Bộ bảo vệ cho dịch vụ Điểm cuối của thiết bị riêng lẻ.</span><span class="sxs-lookup"><span data-stu-id="b9355-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="b9355-105">Tài liệu này báo cáo số lượng thiết bị cần chú ý và giúp bạn xác định các thiết bị gặp sự cố và thực hiện hành động để khắc phục các sự cố đã biết.</span><span class="sxs-lookup"><span data-stu-id="b9355-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="b9355-106">Hai chỉ báo trạng thái trên lát xếp cung cấp thông tin về số lượng thiết bị không báo cáo đúng cách với dịch vụ:</span><span class="sxs-lookup"><span data-stu-id="b9355-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="b9355-107">**Đã cấu hình sai** Các thiết bị có thể báo cáo một phần dữ liệu cảm biến tới Bộ bảo vệ dành cho dịch vụ Điểm cuối và có thể gặp các lỗi về cấu hình cần sửa.</span><span class="sxs-lookup"><span data-stu-id="b9355-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="b9355-108">**Không hoạt động** Các thiết bị đã ngừng báo cáo cho Bộ bảo vệ dành cho dịch vụ Điểm cuối trong hơn bảy ngày trong tháng trước.</span><span class="sxs-lookup"><span data-stu-id="b9355-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="b9355-109">Bấm vào bất kỳ nhóm nào sẽ hướng bạn đến danh sách Thiết bị, được lọc theo lựa chọn của bạn.</span><span class="sxs-lookup"><span data-stu-id="b9355-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="b9355-110">Trên danh sách Thiết bị, bạn có thể lọc danh sách trạng thái theo trạng thái sau đây:</span><span class="sxs-lookup"><span data-stu-id="b9355-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="b9355-111">**Hiện hoạt** Các thiết bị đang tích cực báo cáo cho Bộ bảo vệ dành cho dịch vụ Điểm cuối.</span><span class="sxs-lookup"><span data-stu-id="b9355-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="b9355-112">**Đã cấu hình sai** Các thiết bị có thể báo cáo một phần dữ liệu cảm biến tới Bộ bảo vệ dành cho dịch vụ Điểm cuối nhưng gặp các lỗi về cấu hình cần được sửa.</span><span class="sxs-lookup"><span data-stu-id="b9355-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="b9355-113">Thiết bị bị cấu hình sai có thể có một hoặc một sự cố kết hợp các vấn đề sau đây:</span><span class="sxs-lookup"><span data-stu-id="b9355-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="b9355-114">Không có dữ liệu cảm biến - Thiết bị đã ngừng gửi dữ liệu cảm biến.</span><span class="sxs-lookup"><span data-stu-id="b9355-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="b9355-115">Các cảnh báo giới hạn có thể được kích hoạt từ thiết bị.</span><span class="sxs-lookup"><span data-stu-id="b9355-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="b9355-116">Giao tiếp bị khiếm khuyết - Khả năng giao tiếp với thiết bị suy giảm.</span><span class="sxs-lookup"><span data-stu-id="b9355-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="b9355-117">Gửi tệp để phân tích chuyên sâu, chặn tệp, cách ly thiết bị khỏi mạng và các hành động khác yêu cầu liên lạc với thiết bị có thể không hoạt động.</span><span class="sxs-lookup"><span data-stu-id="b9355-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="b9355-118">**Không hoạt động** Các thiết bị đã ngừng báo cáo với Bộ bảo vệ dành cho dịch vụ Điểm cuối.</span><span class="sxs-lookup"><span data-stu-id="b9355-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="b9355-119">Bạn có thể tải xuống toàn bộ danh sách ở định dạng CSV bằng cách sử dụng tính năng Xuất.</span><span class="sxs-lookup"><span data-stu-id="b9355-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="b9355-120">Để biết thêm thông tin, xem [mục Kiểm tra trạng thái cảm biến trong Bộ bảo vệ Microsoft dành cho Điểm cuối](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="b9355-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="b9355-121">Để biết thêm thông tin về nguyên nhân thiết bị không hoạt động hoặc cấu hình sai, xem mục Khắc phục các cảm biến không tốt trong Bộ bảo [vệ Microsoft dành](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)cho Điểm cuối .</span><span class="sxs-lookup"><span data-stu-id="b9355-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
