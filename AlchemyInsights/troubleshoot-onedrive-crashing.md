---
title: Khắc phục sự cố OneDrive
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826221"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="6c2b3-102">Khắc phục sự cố OneDrive</span><span class="sxs-lookup"><span data-stu-id="6c2b3-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="6c2b3-103">Nếu OneDrive liên tục gặp sự cố, hãy thử các bước khắc phục sự cố sau:</span><span class="sxs-lookup"><span data-stu-id="6c2b3-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="6c2b3-104">**Đảm bảo các phím registry không được đặt:**</span><span class="sxs-lookup"><span data-stu-id="6c2b3-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="6c2b3-105">Sử dụng trình soạn thảo sổ đăng ký, dẫn hướng đến HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="6c2b3-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="6c2b3-106">Nếu giải pháp thay thế là trình bày và đặt thành 1, hãy mở khóa và thay đổi giá trị thành 0.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="6c2b3-107">Khởi động OneDrive theo cách thủ công bằng cách đi đến bắt đầu</span><span class="sxs-lookup"><span data-stu-id="6c2b3-107">Manually launch OneDrive by going to Start</span></span> ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6c2b3-109">, nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6c2b3-110">**Đặt lại OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6c2b3-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="6c2b3-111">Boy</span><span class="sxs-lookup"><span data-stu-id="6c2b3-111">Notes:</span></span>

- <span data-ttu-id="6c2b3-112">Việc đặt lại OneDrive đã ngắt kết nối tất cả các kết nối đồng bộ hiện có của bạn (bao gồm OneDrive cá nhân của bạn nếu thiết lập).</span><span class="sxs-lookup"><span data-stu-id="6c2b3-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="6c2b3-113">Bạn sẽ không mất tệp hoặc dữ liệu bằng cách đặt lại OneDrive trên máy tính của mình.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="6c2b3-114">**Để đặt lại OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="6c2b3-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="6c2b3-115">Mở hộp thoại chạy bằng cách nhấn phím Windows và R.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="6c2b3-116">Nhập% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset và nhấn OK.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="6c2b3-117">Một cửa sổ lệnh có thể xuất hiện một thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="6c2b3-118">Khởi động OneDrive theo cách thủ công bằng cách đi đến bắt đầu</span><span class="sxs-lookup"><span data-stu-id="6c2b3-118">Manually launch OneDrive by going to Start</span></span> ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="6c2b3-120">, nhập OneDrive vào hộp tìm kiếm, rồi bấm vào ứng dụng OneDrive trên máy tính.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="6c2b3-121">Boy</span><span class="sxs-lookup"><span data-stu-id="6c2b3-121">Notes:</span></span>

- <span data-ttu-id="6c2b3-122">Nếu bạn đã chọn chỉ đồng bộ một số thư mục trước khi đặt lại, bạn sẽ cần thực hiện lại sau khi đồng bộ đã hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="6c2b3-123">Đọc [chọn thư mục OneDrive để đồng bộ với máy tính của bạn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)để   biết thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="6c2b3-124">Bạn sẽ cần hoàn thành đối với OneDrive và OneDrive for Business của bạn.</span><span class="sxs-lookup"><span data-stu-id="6c2b3-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>