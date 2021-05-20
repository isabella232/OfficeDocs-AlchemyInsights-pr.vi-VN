---
title: Sự cố với việc loại bỏ thiết bị bị xóa khỏi hoặc không còn sử dụng khỏi Hàng tồn kho Thiết bị
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564614"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="e464f-102">Sự cố với việc loại bỏ thiết bị bị xóa khỏi hoặc không còn sử dụng khỏi Hàng tồn kho Thiết bị</span><span class="sxs-lookup"><span data-stu-id="e464f-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="e464f-103">Bộ bảo vệ Microsoft cho Điểm cuối hiện không cho phép loại bỏ bản ghi thiết bị theo cách thủ công của thiết bị bị xóa khỏi Danh mục Thiết bị.</span><span class="sxs-lookup"><span data-stu-id="e464f-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="e464f-104">Vì mục đích bảo mật, thiết bị vẫn ở trong cổng thông tin dưới dạng bản ghi lịch sử trong tối đa 180 ngày.</span><span class="sxs-lookup"><span data-stu-id="e464f-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="e464f-105">Tuy nhiên, dữ liệu thiết bị sẽ được dọn sạch theo thời gian lưu giữ đã đặt cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="e464f-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="e464f-106">**Lưu ý:** Thiết bị đã xóa khỏi hoặc ngừng hoạt động sẽ tự động chuyển sang trạng **thái Không** hoạt động sau bảy ngày.</span><span class="sxs-lookup"><span data-stu-id="e464f-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="e464f-107">Ngoài ra, thiết bị không hoạt động trong 30 ngày qua không được tính vào dữ liệu phản ánh điểm tiếp cận của tổ chức bạn Quản lý Mối đe dọa và Lỗ hổng điểm tiếp cận cao hoặc Điểm Bảo mật của Microsoft dành cho thiết bị.</span><span class="sxs-lookup"><span data-stu-id="e464f-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="e464f-108">Nếu bạn vẫn không muốn thấy một số thiết bị trong chế độ xem Kiểm kê thiết bị, hãy thử đặt thẻ thiết bị để lọc thiết bị không hoạt động từ chế độ xem Kiểm kê Thiết bị.</span><span class="sxs-lookup"><span data-stu-id="e464f-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="e464f-109">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="e464f-109">For more information, see:</span></span>

[<span data-ttu-id="e464f-110">Các thiết bị ngoài bảng từ Bộ bảo vệ Microsoft dành cho dịch vụ Điểm cuối</span><span class="sxs-lookup"><span data-stu-id="e464f-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="e464f-111">Điểm phơi sáng trong Quản lý Mối đe dọa và Lỗ hổng</span><span class="sxs-lookup"><span data-stu-id="e464f-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="e464f-112">Khắc phục các cảm biến không tốt trong Bộ bảo vệ Microsoft dành cho Điểm cuối</span><span class="sxs-lookup"><span data-stu-id="e464f-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="e464f-113">Cách sử dụng gắn thẻ hiệu quả (Phần 1)</span><span class="sxs-lookup"><span data-stu-id="e464f-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="e464f-114">Cách sử dụng gắn thẻ hiệu quả (Phần 2)</span><span class="sxs-lookup"><span data-stu-id="e464f-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="e464f-115">Cách sử dụng gắn thẻ hiệu quả (Phần 3)</span><span class="sxs-lookup"><span data-stu-id="e464f-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




