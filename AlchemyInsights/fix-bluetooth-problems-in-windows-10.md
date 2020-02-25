---
title: Khắc phục sự cố với Bluetooth trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268715"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="1be6b-102">Khắc phục sự cố với Bluetooth trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="1be6b-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="1be6b-103">Nếu biểu tượng Bluetooth bị thiếu hoặc không thể bật hoặc tắt Bluetooth, bạn có thể muốn chạy bộ hướng dẫn giải quyết trục trặc Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="1be6b-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="1be6b-104">[Mở cài đặt khắc phục sự cố](ms-settings:troubleshoot), bấm **Bluetooth** trong **Tìm và khắc phục sự cố khác**, bấm **chạy bộ hướng dẫn giải quyết trục trặc**.</span><span class="sxs-lookup"><span data-stu-id="1be6b-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="1be6b-105">Nếu bạn không thấy biểu tượng Bluetooth, nhưng Bluetooth xuất hiện trong trình quản lý thiết bị:</span><span class="sxs-lookup"><span data-stu-id="1be6b-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="1be6b-106">Trong trình quản lý thiết bị, bấm **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="1be6b-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="1be6b-107">Nhấn và giữ (hoặc bấm chuột phải vào) tên bộ điều hợp Bluetooth và nhấp vào **gỡ cài đặt thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="1be6b-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="1be6b-108">Tắt thiết bị Windows của bạn, đợi vài giây, và sau đó bật lại.</span><span class="sxs-lookup"><span data-stu-id="1be6b-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="1be6b-109">Windows sẽ cố gắng cài đặt lại trình điều khiển.</span><span class="sxs-lookup"><span data-stu-id="1be6b-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="1be6b-110">Nếu gần đây bạn đã cài đặt các bản cập nhật Windows 10 hoặc nâng cấp lên Windows 10, bạn có thể muốn kiểm tra các bản Cập Nhật trình điều khiển:</span><span class="sxs-lookup"><span data-stu-id="1be6b-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="1be6b-111">Trong quản lý thiết bị, bấm **Bluetooth**, và sau đó nhấp vào tên bộ điều hợp Bluetooth (có thể bao gồm từ "Radio").</span><span class="sxs-lookup"><span data-stu-id="1be6b-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="1be6b-112">Nhấn và giữ (hoặc bấm chuột phải) bộ điều hợp Bluetooth, sau đó bấm **Cập Nhật trình điều khiển** > **Tìm kiếm tự động cho phần mềm trình điều khiển Cập Nhật**.</span><span class="sxs-lookup"><span data-stu-id="1be6b-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="1be6b-113">Làm theo các bước, sau đó nhấp vào **đóng**.</span><span class="sxs-lookup"><span data-stu-id="1be6b-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="1be6b-114">Nếu Windows không thể tìm thấy trình điều khiển Bluetooth mới, hãy truy cập trang web của nhà sản xuất PC và tải xuống trình điều khiển Bluetooth mới nhất từ đó.</span><span class="sxs-lookup"><span data-stu-id="1be6b-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="1be6b-115">Sau khi bạn tải xuống, **bấm Cập Nhật trình điều khiển** >  > **duyệt máy tính của tôi cho phần mềm trình điều khiển\*\*\*\*duyệt** vị trí mà tệp trình điều khiển được lưu trữ > **OK** > **tiếp theo**, và làm theo các bước để cài đặt.</span><span class="sxs-lookup"><span data-stu-id="1be6b-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="1be6b-116">Sau khi cài đặt trình điều khiển Cập Nhật, khởi động lại máy tính, và sau đó kiểm tra xem có khắc phục sự cố kết nối.</span><span class="sxs-lookup"><span data-stu-id="1be6b-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="1be6b-117">Để biết thêm chi tiết về cách khắc phục sự cố Bluetooth, hãy xem toàn bộ bài viết, [khắc phục sự cố Bluetooth trong Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="1be6b-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
