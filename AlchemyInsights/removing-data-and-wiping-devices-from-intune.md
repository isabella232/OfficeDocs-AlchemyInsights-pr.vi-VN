---
title: Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune
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
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701305"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="4c0aa-102">Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune</span><span class="sxs-lookup"><span data-stu-id="4c0aa-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="4c0aa-103">Thiết bị đã rút lui và xóa các hành động từ xa của thiết bị để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện việc đặt lại nhà máy và trả về thiết bị về thiết đặt mặc định của nó.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="4c0aa-104">Đăng nhập vào quản lý thiết bị của Microsoft 365 và đi tới **thiết bị**  >  **tất cả thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="4c0aa-105">Chọn thiết bị bạn muốn xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="4c0aa-106">Chọn loại xóa sạch từ xa mà bạn muốn thực hiện.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="4c0aa-107">Bỏ ẩn chỉ xóa thông tin tổ chức, trong khi toàn bộ khăn lau khôi phục thiết bị về thiết đặt nhà máy.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="4c0aa-108">Chọn **có** để xác nhận.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="4c0aa-109">Cho đến khi hoàn tất việc xóa sạch, trạng thái hành động thiết bị sẽ hiển thị là nghỉ hưu đang chờ xử lý.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="4c0aa-110">Sau khi hoàn thành hành động, bạn sẽ không còn nhìn thấy thiết bị di động trong danh sách thiết bị được quản lý.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="4c0aa-111">**Ghi chú** Không thể loại bỏ dữ liệu công ty khỏi thiết bị đã gia nhập Azure AD.</span><span class="sxs-lookup"><span data-stu-id="4c0aa-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="4c0aa-112">Để biết chi tiết đầy đủ về hiệu ứng của hành động rút lui và xóa sạch, bao gồm những gì được giữ lại và xóa những gì, hãy xem [loại bỏ các thiết bị bằng cách sử dụng quy trình xóa sạch, rút lui hoặc tự hủy đăng ký thiết bị](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="4c0aa-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="4c0aa-113">Để xóa tất cả dữ liệu khỏi thiết bị macOS, hãy xem [xóa tất cả dữ liệu khỏi thiết bị MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="4c0aa-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>