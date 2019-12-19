---
title: Khắc phục sự cố hiện tại màn hình
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738590"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="33039-102">Khắc phục sự cố màn hình hiện có</span><span class="sxs-lookup"><span data-stu-id="33039-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="33039-103">Hãy thử các giải pháp này để khắc phục sự cố màn hình.</span><span class="sxs-lookup"><span data-stu-id="33039-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="33039-104">**Làm mới màn hình hiển thị của bạn:**</span><span class="sxs-lookup"><span data-stu-id="33039-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="33039-105">Nhấn phím sau cùng một lúc: phím Windows + Ctrl + Shift + B. Điều này sẽ làm mới giao tiếp với Driver đồ họa của bạn.</span><span class="sxs-lookup"><span data-stu-id="33039-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="33039-106">Màn hình của bạn sẽ nhấp nháy trong giây lát và trở lại sau vài phút.</span><span class="sxs-lookup"><span data-stu-id="33039-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="33039-107">**Khắc phục sự cố phần cứng màn hình:**</span><span class="sxs-lookup"><span data-stu-id="33039-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="33039-108">Rút cáp kết nối PC của bạn với màn hình và cắm lại.</span><span class="sxs-lookup"><span data-stu-id="33039-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="33039-109">Ngắt kết nối bất kỳ thiết bị không cần thiết nào khỏi PC của bạn (chẳng hạn như bộ điều hợp hoặc bến tàu).</span><span class="sxs-lookup"><span data-stu-id="33039-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="33039-110">**Nếu gần đây bạn đã cài đặt một bản Cập Nhật trên PC, bạn có thể quay lại trình điều khiển màn hình:**</span><span class="sxs-lookup"><span data-stu-id="33039-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="33039-111">Chọn **bắt đầu**, nhập **trình quản lý thiết bị**và chọn **trình quản lý thiết bị** từ kết quả.</span><span class="sxs-lookup"><span data-stu-id="33039-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="33039-112">Mở rộng phần bộ điều hợp **Hiển thị** , bấm chuột phải vào vỉ màn hình của bạn, ands chọn thuộc **tính**.</span><span class="sxs-lookup"><span data-stu-id="33039-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="33039-113">Điều hướng đến tab **trình điều khiển** và chọn **quay lui trình điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="33039-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="33039-114">Lưu ý: nếu không có sẵn hoặc màu xám, hãy chọn **không** từ các tùy chọn bên dưới để chuyển sang bước tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="33039-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="33039-115">Bạn có thể cần phải khởi động lại PC trước khi những thay đổi này có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="33039-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="33039-116">**Gỡ cài đặt và cài đặt lại trình điều khiển hiển thị:**</span><span class="sxs-lookup"><span data-stu-id="33039-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="33039-117">Chọn **bắt đầu**, nhập **trình quản lý thiết bị**và chọn **trình quản lý thiết bị** từ kết quả.</span><span class="sxs-lookup"><span data-stu-id="33039-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="33039-118">Mở rộng phần bộ điều hợp **Hiển thị** , bấm chuột phải vào vỉ màn hình của bạn, ands chọn **thiết bị gỡ cài đặt**.</span><span class="sxs-lookup"><span data-stu-id="33039-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="33039-119">Chọn hộp bên cạnh **xóa phần mềm trình điều khiển cho thiết bị này** và chọn **gỡ cài đặt**.</span><span class="sxs-lookup"><span data-stu-id="33039-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="33039-120">Lưu ý: bạn có thể được yêu cầu khởi động lại máy tính ở giai đoạn này.</span><span class="sxs-lookup"><span data-stu-id="33039-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="33039-121">Hãy chắc chắn để viết xuống các hướng dẫn còn lại trước khi bạn khởi động lại.</span><span class="sxs-lookup"><span data-stu-id="33039-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="33039-122">Mở trình quản lý thiết bị một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="33039-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="33039-123">Mở rộng phần bộ điều hợp **Hiển thị** , bấm chuột phải vào vỉ màn hình của bạn và chọn **Cập Nhật trình điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="33039-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="33039-124">Chọn **tự động tìm kiếm phần mềm trình điều khiển Cập Nhật** và làm theo hướng dẫn cài đặt.</span><span class="sxs-lookup"><span data-stu-id="33039-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>