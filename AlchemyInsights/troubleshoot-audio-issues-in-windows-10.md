---
title: Khắc phục sự cố âm thanh trong Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833313"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="4bb54-102">Khắc phục sự cố âm thanh trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="4bb54-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="4bb54-103">**Chạy trình khắc phục sự cố âm thanh**</span><span class="sxs-lookup"><span data-stu-id="4bb54-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="4bb54-104">Mở [cài đặt khắc phục sự cố](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="4bb54-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="4bb54-105">Chọn **phát âm thanh**  >  **chạy trình** khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="4bb54-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="4bb54-106">**Đặt thiết bị mặc định**</span><span class="sxs-lookup"><span data-stu-id="4bb54-106">**Set the default device**</span></span>

<span data-ttu-id="4bb54-107">Nếu bạn đang kết nối với thiết bị âm thanh bằng cách dùng USB hoặc HDMI, bạn có thể cần đặt thiết bị đó làm mặc định:</span><span class="sxs-lookup"><span data-stu-id="4bb54-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="4bb54-108">Mở   >  **âm thanh** bắt đầu, rồi chọn **âm thanh** hoặc **thay đổi âm thanh hệ thống** từ danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="4bb54-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="4bb54-109">Trên tab **phát lại** , chọn một thiết bị, chọn **đặt mặc định**, rồi chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="4bb54-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="4bb54-110">**Kiểm tra cáp, âm lượng, loa và tai nghe**</span><span class="sxs-lookup"><span data-stu-id="4bb54-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="4bb54-111">Kiểm tra kết nối loa và tai nghe của bạn cho cáp lỏng và đảm bảo rằng chúng được kết nối với đúng Jack.</span><span class="sxs-lookup"><span data-stu-id="4bb54-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="4bb54-112">Kiểm tra mức độ quyền lực và số lượng lớn của bạn, rồi thử chuyển tất cả các điều khiển âm lượng lên.</span><span class="sxs-lookup"><span data-stu-id="4bb54-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="4bb54-113">Một số loa và ứng dụng có điều khiển âm lượng của riêng mình; bạn có thể phải kiểm tra tất cả để đảm bảo rằng họ đang ở đúng mức.</span><span class="sxs-lookup"><span data-stu-id="4bb54-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="4bb54-114">Thử kết nối bằng cách sử dụng cổng USB khác.</span><span class="sxs-lookup"><span data-stu-id="4bb54-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="4bb54-115">**Lưu ý**: Hãy nhớ rằng loa của bạn có thể không hoạt động khi cắm tai nghe.</span><span class="sxs-lookup"><span data-stu-id="4bb54-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="4bb54-116">**Kiểm tra trình quản lý thiết bị**</span><span class="sxs-lookup"><span data-stu-id="4bb54-116">**Check Device Manager**</span></span>

<span data-ttu-id="4bb54-117">Để đảm bảo rằng các trình điều khiển đã Cập Nhật:</span><span class="sxs-lookup"><span data-stu-id="4bb54-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="4bb54-118">Chọn **bắt đầu**, nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** từ danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="4bb54-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="4bb54-119">Bên dưới điều **khiển âm thanh, video và trò chơi**, chọn thẻ âm thanh của bạn, mở nó, chọn tab **trình điều khiển** , rồi chọn **Cập Nhật trình điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="4bb54-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="4bb54-120">**Lưu ý**: nếu Windows không tìm thấy một trình điều khiển mới, hãy tìm kiếm một trên trang web của nhà sản xuất thiết bị và làm theo hướng dẫn của họ.</span><span class="sxs-lookup"><span data-stu-id="4bb54-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="4bb54-121">**Cài đặt lại trình điều khiển**</span><span class="sxs-lookup"><span data-stu-id="4bb54-121">**Reinstall the driver**</span></span>

<span data-ttu-id="4bb54-122">Nếu bạn không thể cập nhật thông qua trình quản lý thiết bị hoặc tìm trình điều khiển mới trên trang web của nhà sản xuất, hãy thử các bước sau:</span><span class="sxs-lookup"><span data-stu-id="4bb54-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="4bb54-123">Trong trình quản lý thiết bị, bấm chuột phải (hoặc nhấn và giữ) trình điều khiển âm thanh, rồi chọn **gỡ cài đặt**.</span><span class="sxs-lookup"><span data-stu-id="4bb54-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="4bb54-124">Khởi động lại thiết bị và Windows sẽ cố cài đặt lại trình điều khiển.</span><span class="sxs-lookup"><span data-stu-id="4bb54-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="4bb54-125">Nếu cài đặt lại trình điều khiển không hoạt động, hãy thử sử dụng trình điều khiển âm thanh chung đi kèm với Windows.</span><span class="sxs-lookup"><span data-stu-id="4bb54-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="4bb54-126">Trong trình quản lý thiết bị, bấm chuột phải (hoặc nhấn và giữ) trình điều khiển âm thanh của bạn > **Cập nhật phần mềm trình điều khiển**  >  **duyệt máy tính của tôi** để  >  **cho tôi chọn từ danh sách trình điều khiển thiết bị trên máy tính của tôi**, chọn **thiết bị âm thanh độ nét cao**, chọn **tiếp theo**, rồi làm theo hướng dẫn để cài đặt nó.</span><span class="sxs-lookup"><span data-stu-id="4bb54-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
