---
title: Tự động dọn dẹp các thiết bị cũ trong InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555739"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="e6dfb-102">Tự động dọn dẹp các thiết bị cũ trong InTune</span><span class="sxs-lookup"><span data-stu-id="e6dfb-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="e6dfb-103">InTune cho phép quản trị viên để cấu hình một khoảng thời gian giữa 90 và 270 ngày, sau đó các thiết bị cũ được loại bỏ khỏi Dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="e6dfb-104">Thiết lập này là tổ chức rộng và một khi kích hoạt đi vào hiệu lực ngay lập tức.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="e6dfb-105">Bất kỳ thiết bị nào không được kiểm tra vào máy chủ InTune trong một khoảng thời gian vượt quá cài đặt sẽ bị xóa vĩnh viễn.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="e6dfb-106">**Lưu ý** Chỉ MDM thiết bị đối tượng đủ điều kiện cho hành động dọn dẹp này.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="e6dfb-107">EAS chỉ đối tượng thiết bị được loại trừ.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="e6dfb-108">Để biết thêm thông tin về khi thiết bị đủ điều kiện để xóa dựa trên cài đặt thiết bị dọn dẹp và "trạng thái":</span><span class="sxs-lookup"><span data-stu-id="e6dfb-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="e6dfb-109">Cài đặt: **xóa thiết bị sau ngày Check-in cuối cùng: có (một số giá trị (N) trong ngày đã chỉ định)**</span><span class="sxs-lookup"><span data-stu-id="e6dfb-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="e6dfb-110">Dựa trên giá trị (N) được cấu hình trong cài đặt, Dịch vụ InTune xoá thiết bị trong những ngày được chỉ định sau khi nó cuối cùng kiểm tra thành công.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="e6dfb-111">Cài đặt: **xóa thiết bị sau ngày nhận phòng cuối cùng: không**</span><span class="sxs-lookup"><span data-stu-id="e6dfb-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="e6dfb-112">180 ngày sau khi chứng chỉ thiết bị hết hạn và không được gia hạn, thiết bị sẽ bị xóa.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="e6dfb-113">**Lưu ý** Trong cả hai trường hợp, thiết bị phải được đăng ký thành công trong InTune.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="e6dfb-114">Đăng ký xảy ra trong thiết bị đầu tiên checkin với dịch vụ InTune.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="e6dfb-115">Nếu thiết bị ghi thành công để InTune nhưng không trở thành InTune đăng ký, thiết bị sẽ bị xóa 270 ngày sau khi đăng ký.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="e6dfb-116">(90 ngày để đánh dấu thiết bị như thu hồi, và sau đó một 180 ngày để xóa hồ sơ.)</span><span class="sxs-lookup"><span data-stu-id="e6dfb-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="e6dfb-117">Không có cơ chế nào tồn tại trong bảng điều khiển InTune để thiết lập ngày hết hạn của chứng nhận thiết bị cho bất kỳ thiết bị nào.</span><span class="sxs-lookup"><span data-stu-id="e6dfb-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>