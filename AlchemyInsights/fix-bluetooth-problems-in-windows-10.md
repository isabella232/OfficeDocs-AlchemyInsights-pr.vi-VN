---
title: Khắc phục sự cố Bluetooth trong Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812954"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="c3404-102">Khắc phục sự cố Bluetooth trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="c3404-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="c3404-103">Nếu biểu tượng Bluetooth bị thiếu hoặc không thể bật hoặc tắt Bluetooth, bạn có thể muốn chạy trình khắc phục sự cố Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="c3404-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="c3404-104">[Mở thiết đặt khắc phục sự cố](ms-settings:troubleshoot), bấm vào **Bluetooth** bên dưới **Tìm và khắc phục các vấn đề khác**, bấm vào **chạy trình** khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="c3404-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="c3404-105">Nếu bạn không nhìn thấy biểu tượng Bluetooth nhưng Bluetooth sẽ xuất hiện trong trình quản lý thiết bị:</span><span class="sxs-lookup"><span data-stu-id="c3404-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="c3404-106">Trong trình quản lý thiết bị, bấm vào **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="c3404-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="c3404-107">Nhấn và giữ (hoặc bấm chuột phải) vào tên bộ điều hợp Bluetooth và bấm **dỡ cài đặt thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="c3404-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="c3404-108">Tắt thiết bị Windows của bạn, chờ vài giây, rồi bật lại.</span><span class="sxs-lookup"><span data-stu-id="c3404-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="c3404-109">Windows sẽ cố cài đặt lại trình điều khiển.</span><span class="sxs-lookup"><span data-stu-id="c3404-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="c3404-110">Nếu gần đây bạn đã cài đặt các bản cập nhật Windows 10 hoặc nâng cấp lên Windows 10, bạn có thể muốn kiểm tra các bản Cập Nhật trình điều khiển:</span><span class="sxs-lookup"><span data-stu-id="c3404-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="c3404-111">Trong trình quản lý thiết bị, bấm **Bluetooth**, rồi bấm vào tên bộ điều hợp Bluetooth (có thể bao gồm từ "Radio").</span><span class="sxs-lookup"><span data-stu-id="c3404-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="c3404-112">Nhấn và giữ (hoặc bấm chuột phải) bộ điều hợp Bluetooth, rồi bấm vào **Cập Nhật tìm kiếm trình điều khiển**  >  **tự động cho phần mềm trình điều khiển đã cập nhật**.</span><span class="sxs-lookup"><span data-stu-id="c3404-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="c3404-113">Làm theo các bước, sau đó bấm **đóng**.</span><span class="sxs-lookup"><span data-stu-id="c3404-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="c3404-114">Nếu Windows không thể tìm thấy một trình điều khiển Bluetooth mới, hãy truy cập trang web của nhà sản xuất PC và tải xuống trình điều khiển Bluetooth mới nhất từ đó.</span><span class="sxs-lookup"><span data-stu-id="c3404-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="c3404-115">Sau khi bạn tải xuống, hãy bấm vào **Cập Nhật trình điều khiển**  >  **duyệt máy tính của tôi để duyệt phần mềm** trình  >  **duyệt** cho vị trí mà các tệp trình điều khiển được lưu trữ > **OK**  >  **tiếp theo**, rồi làm theo các bước để cài đặt.</span><span class="sxs-lookup"><span data-stu-id="c3404-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="c3404-116">Sau khi cài đặt trình điều khiển đã cập nhật, hãy khởi động lại máy, rồi kiểm tra xem khắc phục sự cố kết nối hay không.</span><span class="sxs-lookup"><span data-stu-id="c3404-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="c3404-117">Để biết thêm chi tiết về cách khắc phục sự cố Bluetooth, vui lòng xem bài viết đầy đủ, [khắc phục các vấn đề về Bluetooth trong Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="c3404-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
