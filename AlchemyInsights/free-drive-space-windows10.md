---
title: Giải phóng dung lượng ổ đĩa trong Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505378"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="d415b-102">Giải phóng dung lượng ổ đĩa trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="d415b-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="d415b-103">Dưới đây là hai tùy chọn để giải phóng dung lượng ổ đĩa trong Windows:</span><span class="sxs-lookup"><span data-stu-id="d415b-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="d415b-104">Giải phóng dung lượng ổ đĩa trong Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d415b-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="d415b-105">Giải phóng dung lượng cho các bản cập nhật Windows 10 với thiết bị lưu trữ bên ngoài.</span><span class="sxs-lookup"><span data-stu-id="d415b-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="d415b-106">Nếu bạn vẫn có dung lượng ổ đĩa thấp sau khi sử dụng dọn dẹp ổ đĩa, có thể là thư mục TEMP của bạn sẽ nhanh chóng được điền với các tệp ứng dụng (. appx) được Microsoft Store sử dụng.</span><span class="sxs-lookup"><span data-stu-id="d415b-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="d415b-107">Để khắc phục sự cố này, hãy đặt lại cửa hàng, xóa bộ đệm ẩn lưu trữ, sau đó chạy trình khắc phục sự cố Windows Update.</span><span class="sxs-lookup"><span data-stu-id="d415b-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="d415b-108">Đảm bảo rằng Microsoft Store sẽ được đóng lại trước khi bạn tiếp tục thực hiện các bước này.</span><span class="sxs-lookup"><span data-stu-id="d415b-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="d415b-109">**Bước 1: đặt lại Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="d415b-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="d415b-110">**Ghi chú** Việc này sẽ xóa vĩnh viễn dữ liệu ứng dụng trên thiết bị, bao gồm các tùy chọn và chi tiết đăng nhập của bạn.</span><span class="sxs-lookup"><span data-stu-id="d415b-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="d415b-111">Chọn thiết đặt **bắt đầu** ứng dụng  >    >  **ứng** dụng  >  **& các tính năng**.</span><span class="sxs-lookup"><span data-stu-id="d415b-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="d415b-112">Trong danh sách ứng dụng, định vị và chọn Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d415b-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="d415b-113">Chọn **tùy chọn nâng cao**.</span><span class="sxs-lookup"><span data-stu-id="d415b-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="d415b-114">Cuộn xuống và chọn **đặt lại**, rồi **xác nhận đặt lại**.</span><span class="sxs-lookup"><span data-stu-id="d415b-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="d415b-115">**Bước 2: xóa bộ đệm ẩn Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="d415b-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="d415b-116">Nhấn phím logo Windows + R để mở hộp thoại chạy.</span><span class="sxs-lookup"><span data-stu-id="d415b-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="d415b-117">Nhập wsreset.exe và chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="d415b-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="d415b-118">Cửa sổ dấu nhắc lệnh trống mở ra.</span><span class="sxs-lookup"><span data-stu-id="d415b-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="d415b-119">Sau khoảng 10 giây, cửa sổ sẽ đóng lại và cửa hàng mở ra tự động.</span><span class="sxs-lookup"><span data-stu-id="d415b-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="d415b-120">**Bước 3: đặt lại Windows Update**</span><span class="sxs-lookup"><span data-stu-id="d415b-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="d415b-121">Chọn **bắt đầu**  >    >  **Cập Nhật** cài đặt &  >  **khắc phục sự cố** bảo mật.</span><span class="sxs-lookup"><span data-stu-id="d415b-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="d415b-122">Cuộn xuống và chọn **Windows Update** từ danh sách, rồi chọn **chạy trình** khắc phục sự cố.</span><span class="sxs-lookup"><span data-stu-id="d415b-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="d415b-123">Khởi động lại máy tính của bạn và kiểm tra xem bạn vẫn đang gặp sự cố.</span><span class="sxs-lookup"><span data-stu-id="d415b-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

