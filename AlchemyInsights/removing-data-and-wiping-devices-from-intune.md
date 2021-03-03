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
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416335"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="f1e93-102">Loại bỏ dữ liệu và các thiết bị xóa khỏi InTune</span><span class="sxs-lookup"><span data-stu-id="f1e93-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="f1e93-103">Thiết bị đã rút lui và xóa các hành động từ xa của thiết bị để loại bỏ dữ liệu công ty được quản lý bởi InTune hoặc để thực hiện việc đặt lại nhà máy và trả về thiết bị về thiết đặt mặc định của nó.</span><span class="sxs-lookup"><span data-stu-id="f1e93-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="f1e93-104">Đăng nhập vào quản lý thiết bị của Microsoft 365 và đi tới **thiết bị**  >  **tất cả thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="f1e93-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="f1e93-105">Chọn thiết bị bạn muốn xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="f1e93-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="f1e93-106">Chọn loại xóa sạch từ xa mà bạn muốn thực hiện.</span><span class="sxs-lookup"><span data-stu-id="f1e93-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="f1e93-107">Bỏ ẩn chỉ xóa thông tin tổ chức, trong khi toàn bộ khăn lau khôi phục thiết bị về thiết đặt nhà máy.</span><span class="sxs-lookup"><span data-stu-id="f1e93-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="f1e93-108">Chọn **có** để xác nhận.</span><span class="sxs-lookup"><span data-stu-id="f1e93-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="f1e93-109">Cho đến khi hoàn tất việc xóa sạch, trạng thái hành động thiết bị sẽ hiển thị là *nghỉ hưu đang chờ xử* lý.</span><span class="sxs-lookup"><span data-stu-id="f1e93-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="f1e93-110">Sau khi hoàn thành hành động, bạn sẽ không còn nhìn thấy thiết bị di động trong danh sách thiết bị được quản lý.</span><span class="sxs-lookup"><span data-stu-id="f1e93-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="f1e93-111">Không thể loại bỏ dữ liệu công ty khỏi thiết bị đã gia nhập Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f1e93-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="f1e93-112">Để biết chi tiết đầy đủ về hiệu ứng của hành động rút lui và xóa sạch, bao gồm những gì được giữ lại và xóa những gì, hãy xem tài liệu hướng dẫn sau:</span><span class="sxs-lookup"><span data-stu-id="f1e93-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="f1e93-113">[Loại bỏ các thiết bị bằng cách sử dụng quy trình xóa sạch, rút lui hoặc bỏ đăng ký theo cách thủ công thiết bị](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="f1e93-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="f1e93-114">Làm thế nào để chỉ xóa dữ liệu công ty từ các ứng dụng được quản lý trên InTune</span><span class="sxs-lookup"><span data-stu-id="f1e93-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="f1e93-115">[Xóa tất cả dữ liệu khỏi thiết bị macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="f1e93-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>