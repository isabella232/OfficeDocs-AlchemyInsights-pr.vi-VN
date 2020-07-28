---
title: Xóa dữ liệu và xóa các thiết bị khỏi InTune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440461"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="a2c8d-102">Xóa dữ liệu và xóa các thiết bị khỏi InTune</span><span class="sxs-lookup"><span data-stu-id="a2c8d-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="a2c8d-103">Các thiết bị nghỉ hưu và xóa thiết bị hành động từ xa có thể được sử dụng để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện một Factory Reset và trả lại thiết bị về cài đặt mặc định của nó.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="a2c8d-104">Đăng nhập vào Microsoft 365 quản lý thiết bị, và đi đến **thiết**bị  >  **tất cả các thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="a2c8d-105">Chọn thiết bị bạn muốn xóa.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="a2c8d-106">Chọn loại xóa từ xa mà bạn muốn thực hiện.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="a2c8d-107">Nghỉ hưu chỉ xoá thông tin tổ chức, trong khi khăn lau đầy đủ khôi phục thiết bị về cài đặt gốc của nó.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="a2c8d-108">Chọn **có** để xác nhận.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="a2c8d-109">Cho đến khi kết thúc sạch, trạng thái hành động của thiết bị hiển thị là đang chờ xử lý.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="a2c8d-110">Sau khi hoàn tất hành động, bạn sẽ không còn thấy thiết bị di động trong danh sách thiết bị được quản lý.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="a2c8d-111">**Lưu ý** Không thể xóa dữ liệu công ty khỏi các thiết bị đã tham gia vào Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a2c8d-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="a2c8d-112">Để biết chi tiết đầy đủ về hiệu quả của các hành động về hưu và xóa, bao gồm cả những gì được giữ lại và những gì bị xóa, xem [loại bỏ các thiết bị bằng cách sử dụng xóa sạch, rút lui hoặc tự unenrolling thiết bị](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="a2c8d-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="a2c8d-113">Để xóa tất cả dữ liệu khỏi thiết bị macOS, xem [xóa tất cả dữ liệu khỏi thiết bị MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="a2c8d-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>