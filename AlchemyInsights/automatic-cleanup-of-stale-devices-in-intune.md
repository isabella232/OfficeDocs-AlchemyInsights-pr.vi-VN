---
title: Tự động dọn dẹp các thiết bị cũ trong InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715043"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="45af4-102">Tự động dọn dẹp các thiết bị cũ trong InTune</span><span class="sxs-lookup"><span data-stu-id="45af4-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="45af4-103">InTune cho phép người quản trị cấu hình khoảng thời gian giữa 90 và 270 ngày, sau khi các thiết bị cũ được loại bỏ khỏi Dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="45af4-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="45af4-104">Thiết đặt này là tổ chức rộng và đã kích hoạt một lần sẽ có hiệu lực ngay lập tức.</span><span class="sxs-lookup"><span data-stu-id="45af4-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="45af4-105">Mọi thiết bị không được kiểm nhập vào máy chủ InTune trong một khoảng thời gian vượt quá thiết đặt sẽ bị xóa vĩnh viễn.</span><span class="sxs-lookup"><span data-stu-id="45af4-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="45af4-106">**Ghi chú** Chỉ các đối tượng thiết bị MDM đủ điều kiện cho hành động dọn dẹp này.</span><span class="sxs-lookup"><span data-stu-id="45af4-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="45af4-107">Chỉ các đối tượng của thiết bị EAS được loại trừ.</span><span class="sxs-lookup"><span data-stu-id="45af4-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="45af4-108">Để biết thêm thông tin về khi thiết bị trở nên đủ điều kiện để xóa căn cứ theo thiết đặt thiết bị dọn dẹp và trạng thái "của bạn":</span><span class="sxs-lookup"><span data-stu-id="45af4-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="45af4-109">Thiết đặt: **xóa các thiết bị sau ngày kiểm nhập lần cuối: có (một số giá trị (N) trong các ngày đã xác định)**</span><span class="sxs-lookup"><span data-stu-id="45af4-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="45af4-110">Dựa trên giá trị (N) được đặt cấu hình trong thiết đặt, Dịch vụ InTune sẽ xóa thiết bị trong những ngày cụ thể sau khi kiểm tra thành công lần cuối.</span><span class="sxs-lookup"><span data-stu-id="45af4-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="45af4-111">Thiết đặt:  **xóa các thiết bị sau ngày kiểm nhập lần cuối: không có**</span><span class="sxs-lookup"><span data-stu-id="45af4-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="45af4-112">180 ngày sau khi chứng chỉ thiết bị hết hạn và không được gia hạn, thiết bị sẽ bị xóa.</span><span class="sxs-lookup"><span data-stu-id="45af4-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="45af4-113">**Ghi chú** Trong cả hai trường hợp, thiết bị phải được đăng ký thành công trong InTune.</span><span class="sxs-lookup"><span data-stu-id="45af4-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="45af4-114">Đăng ký xảy ra trong trình kiểm tra thiết bị đầu tiên với dịch vụ InTune.</span><span class="sxs-lookup"><span data-stu-id="45af4-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="45af4-115">Nếu thiết bị đã được thực hiện thành công với InTune nhưng không trở thành InTune đã đăng ký, thiết bị sẽ bị xóa 270 ngày sau khi ghi danh.</span><span class="sxs-lookup"><span data-stu-id="45af4-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="45af4-116">(90 ngày để đánh dấu thiết bị là thu hồi, rồi sau đó 180 ngày khác để xóa bản ghi.)</span><span class="sxs-lookup"><span data-stu-id="45af4-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="45af4-117">Không có cơ chế hiện tại trong giao diện điều khiển InTune để thiết lập ngày hết hạn của chứng chỉ thiết bị cho bất kỳ thiết bị nào đã cho.</span><span class="sxs-lookup"><span data-stu-id="45af4-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>