---
title: Nguồn điện hoặc biểu tượng pin bị thiếu trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: d82994c86126ea9c789e846a74e03794c32c5c3c
ms.sourcegitcommit: b398afd92d4259f893c25b48aec65921e6cc68d6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/16/2020
ms.locfileid: "44269521"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="e5730-102">Nguồn điện hoặc biểu tượng pin bị thiếu trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="e5730-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="e5730-103">Nếu thiết bị chạy Windows 10 của bạn có pin (ví dụ: máy tính xách tay hoặc máy tính bảng hoặc PC kết nối qua USB với một UPS), thông thường một biểu tượng nguồn/pin được hiển thị trong thanh tác vụ gần đồng hồ, ví dụ:</span><span class="sxs-lookup"><span data-stu-id="e5730-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Biểu tượng pin](media/battery-icon.png)

<span data-ttu-id="e5730-105">Nếu bạn không thấy biểu tượng này, nó có thể bị ẩn:</span><span class="sxs-lookup"><span data-stu-id="e5730-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="e5730-106">Đi tới **[cài đặt > cá nhân hóa > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="e5730-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="e5730-107">Trong khu vực thông báo, bấm **chọn các biểu tượng xuất hiện trên thanh tác vụ**.</span><span class="sxs-lookup"><span data-stu-id="e5730-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="e5730-108">Sau đó tìm mục **Power** trong danh sách và chuyển đổi cài đặt của nó thành **bật**.</span><span class="sxs-lookup"><span data-stu-id="e5730-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Hiển thị biểu tượng nguồn điện trong thanh tác vụ](media/power-icon-on.png)

<span data-ttu-id="e5730-110">**Troubleshooting**</span><span class="sxs-lookup"><span data-stu-id="e5730-110">**Troubleshooting**</span></span>

<span data-ttu-id="e5730-111">Nếu bạn đã làm theo các hướng dẫn ở trên và bật tắt **nguồn** màu xám hoặc không hiển thị, trong hộp tìm kiếm trên thanh tác vụ, hãy nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** trong danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="e5730-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="e5730-112">Trong **pin**, bấm chuột phải vào pin cho thiết bị của bạn, bấm **vô hiệu hoá**và bấm **có**.</span><span class="sxs-lookup"><span data-stu-id="e5730-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="e5730-113">Chờ một vài giây, và sau đó nhấp chuột phải vào pin và **kích hoạt**.</span><span class="sxs-lookup"><span data-stu-id="e5730-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="e5730-114">Sau đó khởi động lại thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="e5730-114">Then restart your device.</span></span>

<span data-ttu-id="e5730-115">Nếu bạn làm theo các hướng dẫn ở trên, nhưng biểu tượng pin không xuất hiện trên thanh tác vụ, trong hộp tìm kiếm trên thanh tác vụ, gõ **Task Manager**, và sau đó nhấp vào **Task Manager** trong danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="e5730-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="e5730-116">Trên tab **quy trình** , trong **tên**, bấm chuột phải vào **Explorer**, và sau đó bấm **khởi động lại**.</span><span class="sxs-lookup"><span data-stu-id="e5730-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
