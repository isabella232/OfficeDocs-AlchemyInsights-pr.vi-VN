---
title: Khắc phục sự cố OneDrive sập
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749243"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="b1ce4-102">Khắc phục sự cố OneDrive sập</span><span class="sxs-lookup"><span data-stu-id="b1ce4-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="b1ce4-103">Nếu OneDrive liên tục sập, hãy thử các bước khắc phục sự cố sau:</span><span class="sxs-lookup"><span data-stu-id="b1ce4-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="b1ce4-104">**Đảm bảo khoá đăng ký không thiết lập:**</span><span class="sxs-lookup"><span data-stu-id="b1ce4-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="b1ce4-105">Sử dụng Registry Editor, điều hướng đến HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="b1ce4-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="b1ce4-106">Nếu DisableFileSyncNGSC có và đặt thành 1, mở khoá và thay đổi giá trị thành 0.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="b1ce4-107">Khởi chạy bằng tay OneDrive bằng cách đi tới bắt đầu</span><span class="sxs-lookup"><span data-stu-id="b1ce4-107">Manually launch OneDrive by going to Start</span></span> ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="b1ce4-109">, nhập OneDrive vào hộp tìm kiếm rồi bấm vào ứng dụng OneDrive dành cho máy tính để bàn.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="b1ce4-110">**Đặt lại OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="b1ce4-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="b1ce4-111">Ghi chú:</span><span class="sxs-lookup"><span data-stu-id="b1ce4-111">Notes:</span></span>

- <span data-ttu-id="b1ce4-112">Việc đặt lại OneDrive ngắt kết nối tất cả các kết nối đồng bộ hiện có của bạn (bao gồm OneDrive cá nhân của bạn nếu thiết lập).</span><span class="sxs-lookup"><span data-stu-id="b1ce4-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="b1ce4-113">Bạn sẽ không mất tệp hoặc dữ liệu bằng việc đặt lại OneDrive trên máy tính của mình.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="b1ce4-114">**Để đặt lại OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="b1ce4-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="b1ce4-115">Mở hộp thoại chạy bằng cách nhấn phím Windows và R.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="b1ce4-116">Nhập% LocalAppData% \Microsoft\OneDrive\onedrive.exe/Reset và nhấn OK.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="b1ce4-117">Một cửa sổ lệnh có thể xuất hiện một thời gian ngắn.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="b1ce4-118">Khởi chạy bằng tay OneDrive bằng cách đi tới bắt đầu</span><span class="sxs-lookup"><span data-stu-id="b1ce4-118">Manually launch OneDrive by going to Start</span></span> ![Nhấn phím Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="b1ce4-120">, nhập OneDrive vào hộp tìm kiếm rồi bấm vào ứng dụng OneDrive dành cho máy tính để bàn.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="b1ce4-121">Ghi chú:</span><span class="sxs-lookup"><span data-stu-id="b1ce4-121">Notes:</span></span>

- <span data-ttu-id="b1ce4-122">Nếu bạn đã chọn để đồng bộ chỉ một số thư mục trước khi đặt lại, bạn sẽ cần phải làm điều đó một lần nữa đồng bộ đã hoàn thành.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="b1ce4-123">Đọc [chọn thư mục OneDrive để đồng bộ hóa với máy tính của bạn](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)để biết   thêm thông tin.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="b1ce4-124">Bạn sẽ cần hoàn tất việc này cho OneDrive và OneDrive dành cho doanh nghiệp cá nhân của mình.</span><span class="sxs-lookup"><span data-stu-id="b1ce4-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>