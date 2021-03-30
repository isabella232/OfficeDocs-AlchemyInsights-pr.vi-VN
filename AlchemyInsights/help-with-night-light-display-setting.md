---
title: Trợ giúp với thiết đặt hiển thị ánh sáng đêm
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405186"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="39801-102">Trợ giúp với thiết đặt hiển thị ánh sáng đêm</span><span class="sxs-lookup"><span data-stu-id="39801-102">Help with the night light display setting</span></span>

<span data-ttu-id="39801-103">Để tìm hiểu thêm về thiết đặt hiển thị thời gian ban đêm, hãy xem [thiết đặt màn hình hiển thị của bạn cho thời gian ban đêm trong Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="39801-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="39801-104">Nếu các tùy chọn ánh sáng ban đêm được tô xám trong thiết đặt, hãy kiểm tra trình điều khiển hiển thị của bạn:</span><span class="sxs-lookup"><span data-stu-id="39801-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="39801-105">Bấm vào hộp tìm kiếm trên thanh tác vụ và nhập **trình quản lý thiết bị**, rồi chọn **trình quản lý thiết bị** trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="39801-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="39801-106">Bung rộng bộ điều hợp **Hiển thị**.</span><span class="sxs-lookup"><span data-stu-id="39801-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="39801-107">Rất tiếc, tính năng đêm chiếu sáng không sẵn dùng nếu thiết bị của bạn sử dụng trình điều khiển DisplayLink hoặc trình điều khiển hiển thị cơ bản.</span><span class="sxs-lookup"><span data-stu-id="39801-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="39801-108">Tính năng chiếu sáng ban đêm làm cho việc sử dụng công nghệ đồ họa gần đây, vì vậy bạn có thể cần cập nhật trình điều khiển hiển thị của mình:</span><span class="sxs-lookup"><span data-stu-id="39801-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="39801-109">Kiểm tra các bản Cập Nhật bằng cách đi đến **bắt đầu**  >  Cập Nhật **cài đặt**  >  **& bảo mật**  >  **Windows Update**  >  **kiểm tra Cập Nhật**.</span><span class="sxs-lookup"><span data-stu-id="39801-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="39801-110">HAY</span><span class="sxs-lookup"><span data-stu-id="39801-110">OR</span></span>

- <span data-ttu-id="39801-111">Truy nhập trang web hỗ trợ của nhà sản xuất phần cứng để tải xuống theo cách thủ công và cài đặt trình điều khiển hiển thị mới nhất.</span><span class="sxs-lookup"><span data-stu-id="39801-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="39801-112">Đặt lại ánh sáng đêm trong sổ đăng ký</span><span class="sxs-lookup"><span data-stu-id="39801-112">Reset night light in the registry</span></span>

<span data-ttu-id="39801-113">Nếu Cập Nhật trình điều khiển hiển thị của bạn không hoạt động, bạn có thể cần đặt lại ánh sáng đêm trong sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="39801-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="39801-114">**Thận trọng:** Bước khắc phục sự cố này chỉ được đề xuất dành cho người dùng nâng cao.</span><span class="sxs-lookup"><span data-stu-id="39801-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="39801-115">Các vấn đề nghiêm trọng có thể xảy ra nếu bạn sửa đổi không chính xác của sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="39801-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="39801-116">Để được thêm bảo vệ, hãy sao lưu sổ đăng ký trước khi bạn sửa đổi để bạn có thể khôi phục nó nếu vấn đề xảy ra.</span><span class="sxs-lookup"><span data-stu-id="39801-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="39801-117">Trong hộp tìm kiếm, nhập **regedit**, rồi chọn **trình soạn thảo sổ đăng ký** trong kết quả tìm kiếm.</span><span class="sxs-lookup"><span data-stu-id="39801-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="39801-118">Đi đến khóa đăng ký sau đây:</span><span class="sxs-lookup"><span data-stu-id="39801-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="39801-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="39801-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="39801-120">Xuất và sau đó xóa khóa phụ sau đây: $ $windows. Data. bluelightreduction. bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="39801-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="39801-121">Xuất và sau đó xóa khóa phụ sau đây: $ $windows. Data. bluelightreduction. Settings</span><span class="sxs-lookup"><span data-stu-id="39801-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="39801-122">Khởi động lại Windows và xác nhận xem tùy chọn ánh sáng đêm sẵn dùng.</span><span class="sxs-lookup"><span data-stu-id="39801-122">Restart Windows and verify if the night light options are available.</span></span>


