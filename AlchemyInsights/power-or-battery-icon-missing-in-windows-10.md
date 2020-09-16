---
title: Mất điện hoặc biểu tượng pin trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 10213843f8ec5ceeaa191d3373406d767f2bea3c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771563"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="f4407-102">Mất điện hoặc biểu tượng pin trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="f4407-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="f4407-103">Nếu thiết bị chạy Windows 10 của bạn có pin (ví dụ, máy tính xách tay hoặc máy tính bảng hoặc PC được kết nối qua cổng USB đến một UPS), thường là biểu tượng Power/Battery được hiển thị trong thanh tác vụ gần đồng hồ, ví dụ:</span><span class="sxs-lookup"><span data-stu-id="f4407-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Biểu tượng pin](media/battery-icon.png)

<span data-ttu-id="f4407-105">Nếu bạn không nhìn thấy biểu tượng này, có thể bạn sẽ bị ẩn:</span><span class="sxs-lookup"><span data-stu-id="f4407-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="f4407-106">Đi đến **[cài đặt > thanh tác vụ > cá](ms-settings:taskbar?activationSource=GetHelp)** nhân hóa.</span><span class="sxs-lookup"><span data-stu-id="f4407-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="f4407-107">Trong khu vực thông báo, hãy bấm **chọn biểu tượng nào xuất hiện trên thanh tác vụ**.</span><span class="sxs-lookup"><span data-stu-id="f4407-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="f4407-108">Sau đó tìm mục **Power** trong danh sách và chuyển đổi thiết đặt thành **bật**.</span><span class="sxs-lookup"><span data-stu-id="f4407-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Hiển thị biểu tượng Power trong thanh tác vụ](media/power-icon-on.png)

<span data-ttu-id="f4407-110">**Giải**</span><span class="sxs-lookup"><span data-stu-id="f4407-110">**Troubleshooting**</span></span>

<span data-ttu-id="f4407-111">Nếu bạn đã làm theo các hướng dẫn trên và bật tắt của **Power** sẽ bị mờ đi hoặc không nhìn thấy được, trong hộp tìm kiếm trên thanh tác vụ, hãy nhập **trình quản lý thiết bị**, rồi chọn **Device Manager** trong danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="f4407-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="f4407-112">Bên dưới **pin**, bấm chuột phải vào pin cho thiết bị của bạn, bấm vào **tắt**, rồi bấm **có**.</span><span class="sxs-lookup"><span data-stu-id="f4407-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="f4407-113">Chờ vài giây, rồi bấm chuột phải vào pin và bấm **bật**.</span><span class="sxs-lookup"><span data-stu-id="f4407-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="f4407-114">Sau đó khởi động lại thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="f4407-114">Then restart your device.</span></span>

<span data-ttu-id="f4407-115">Nếu bạn đã làm theo các hướng dẫn ở trên, nhưng biểu tượng pin không xuất hiện trên thanh tác vụ, trong hộp tìm kiếm trên thanh tác vụ, hãy gõ **trình quản lý tác vụ**, rồi bấm **trình quản lý tác vụ** trong danh sách kết quả.</span><span class="sxs-lookup"><span data-stu-id="f4407-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="f4407-116">Trên tab **tiến trình** , bên dưới **tên**, hãy bấm chuột phải vào **Explorer**, rồi bấm vào **khởi động lại**.</span><span class="sxs-lookup"><span data-stu-id="f4407-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
