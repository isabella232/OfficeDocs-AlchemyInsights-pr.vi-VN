---
title: Khắc phục sự cố màn hình hiện có
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690733"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="d1b10-102">Khắc phục sự cố màn hình hiện có</span><span class="sxs-lookup"><span data-stu-id="d1b10-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="d1b10-103">Hãy thử các giải pháp này để khắc phục sự cố màn hình.</span><span class="sxs-lookup"><span data-stu-id="d1b10-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="d1b10-104">**Làm mới màn hình hiển thị của bạn:**</span><span class="sxs-lookup"><span data-stu-id="d1b10-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="d1b10-105">Nhấn các phím sau đây cùng một lúc: phím Windows + Ctrl + Shift + B. Điều này sẽ làm mới liên lạc với trình điều khiển đồ họa của bạn.</span><span class="sxs-lookup"><span data-stu-id="d1b10-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="d1b10-106">Màn hình của bạn sẽ được khắc phục trong giây lát và trở lại sau vài giây.</span><span class="sxs-lookup"><span data-stu-id="d1b10-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="d1b10-107">**Khắc phục sự cố phần cứng theo dõi:**</span><span class="sxs-lookup"><span data-stu-id="d1b10-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="d1b10-108">Tháo cáp kết nối PC của bạn với màn hình của bạn, rồi cắm lại vào đó.</span><span class="sxs-lookup"><span data-stu-id="d1b10-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="d1b10-109">Ngắt kết nối bất kỳ thiết bị không cần thiết nào từ PC của bạn (chẳng hạn như adapter hoặc Docks).</span><span class="sxs-lookup"><span data-stu-id="d1b10-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="d1b10-110">**Nếu gần đây bạn đã cài đặt bản Cập Nhật trên PC của mình, bạn có thể cuộn ngược lại trình điều khiển hiển thị của mình:**</span><span class="sxs-lookup"><span data-stu-id="d1b10-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="d1b10-111">Chọn **bắt đầu**, nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** từ kết quả.</span><span class="sxs-lookup"><span data-stu-id="d1b10-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d1b10-112">Bung rộng phần bộ điều hợp **Hiển thị** , bấm chuột phải vào bộ điều hợp Hiển thị của bạn, bỏ chọn **thuộc tính**.</span><span class="sxs-lookup"><span data-stu-id="d1b10-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="d1b10-113">Dẫn hướng đến tab **trình điều khiển** , rồi chọn **cuộn lại trình điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="d1b10-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="d1b10-114">Lưu ý: nếu điều này không sẵn dùng hoặc bị xám, hãy chọn **không** có từ các tùy chọn bên dưới để chuyển đến bước tiếp theo.</span><span class="sxs-lookup"><span data-stu-id="d1b10-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="d1b10-115">Bạn có thể cần phải khởi động lại PC của bạn trước khi những thay đổi này có hiệu lực.</span><span class="sxs-lookup"><span data-stu-id="d1b10-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="d1b10-116">**Gỡ cài đặt và cài đặt lại trình điều khiển hiển thị:**</span><span class="sxs-lookup"><span data-stu-id="d1b10-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="d1b10-117">Chọn **bắt đầu**, nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** từ kết quả.</span><span class="sxs-lookup"><span data-stu-id="d1b10-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d1b10-118">Bung rộng phần bộ điều hợp **Hiển thị** , bấm chuột phải vào bộ điều hợp Hiển thị, chọn **gỡ cài đặt thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="d1b10-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="d1b10-119">Chọn hộp bên cạnh **xóa phần mềm trình điều khiển cho thiết bị này** , rồi chọn **gỡ cài đặt**.</span><span class="sxs-lookup"><span data-stu-id="d1b10-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="d1b10-120">Lưu ý: bạn có thể được yêu cầu khởi động lại máy tính của bạn ở giai đoạn này.</span><span class="sxs-lookup"><span data-stu-id="d1b10-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="d1b10-121">Hãy đảm bảo bạn ghi các hướng dẫn còn lại trước khi khởi động lại.</span><span class="sxs-lookup"><span data-stu-id="d1b10-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="d1b10-122">Mở lại trình quản lý thiết bị.</span><span class="sxs-lookup"><span data-stu-id="d1b10-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="d1b10-123">Bung rộng phần **Hiển thị adapter** , bấm chuột phải vào bộ điều hợp Hiển thị của bạn, rồi chọn **Cập Nhật trình điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="d1b10-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="d1b10-124">Chọn **Tìm kiếm tự động để cập nhật phần mềm trình điều khiển** và làm theo hướng dẫn cài đặt.</span><span class="sxs-lookup"><span data-stu-id="d1b10-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>