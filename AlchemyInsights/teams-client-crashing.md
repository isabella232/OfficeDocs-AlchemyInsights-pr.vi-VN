---
title: Đội khách hàng bị rơi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354076"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="c9f95-102">Đội khách hàng bị rơi?</span><span class="sxs-lookup"><span data-stu-id="c9f95-102">Teams client crashing?</span></span>

<span data-ttu-id="c9f95-103">Nếu khách hàng teams của bạn bị sập, hãy thử các cách sau:</span><span class="sxs-lookup"><span data-stu-id="c9f95-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="c9f95-104">Nếu bạn đang sử dụng ứng dụng teams trên máy tính để bàn, hãy đảm [bảo rằng ứng dụng được Cập Nhật hoàn toàn](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="c9f95-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="c9f95-105">Đảm bảo rằng tất cả các [URL của Microsoft 365 và phạm vi địa chỉ](https://docs.microsoft.com/microsoftteams/connectivity-issues) có thể truy cập.</span><span class="sxs-lookup"><span data-stu-id="c9f95-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="c9f95-106">Đăng nhập bằng tài khoản quản trị viên của bạn và kiểm tra [bảng điều khiển dịch vụ y tế](https://docs.microsoft.com/office365/enterprise/view-service-health) để xác minh rằng không có sự cố hỏng hóc hoặc dịch vụ tồn tại.</span><span class="sxs-lookup"><span data-stu-id="c9f95-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="c9f95-107">Gỡ cài đặt và cài đặt lại ứng dụng teams (liên kết)</span><span class="sxs-lookup"><span data-stu-id="c9f95-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="c9f95-108">Duyệt đến thư mục%appdata%\Microsoft\teams\ trên máy tính của bạn và xoá tất cả các tệp trong thư mục đó.</span><span class="sxs-lookup"><span data-stu-id="c9f95-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="c9f95-109">[Tải xuống và cài đặt ứng dụng teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)và nếu có thể, hãy cài đặt teams làm quản trị viên (nhấp chuột phải vào trình cài đặt teams và chọn "chạy với tư vị người quản trị" nếu có).</span><span class="sxs-lookup"><span data-stu-id="c9f95-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="c9f95-110">Nếu khách hàng teams của bạn vẫn bị sập, bạn có thể tạo lại sự cố không?</span><span class="sxs-lookup"><span data-stu-id="c9f95-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="c9f95-111">Nếu có:</span><span class="sxs-lookup"><span data-stu-id="c9f95-111">If so:</span></span>

1. <span data-ttu-id="c9f95-112">Sử dụng trình ghi bước để nắm bắt các bước của bạn.</span><span class="sxs-lookup"><span data-stu-id="c9f95-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="c9f95-113">Đóng tất cả các ứng dụng không cần thiết hoặc bí mật.</span><span class="sxs-lookup"><span data-stu-id="c9f95-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="c9f95-114">Khởi động trình ghi bước và tái tạo sự cố khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="c9f95-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="c9f95-115">[Thu thập các đội ghi mà nắm bắt các bước Create ghi lại](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="c9f95-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="c9f95-116">**Lưu ý**: đảm bảo bạn chụp địa chỉ đăng nhập của người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="c9f95-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="c9f95-117">Thu thập các bãi chứa và/hoặc thông tin Xô lỗi (Windows).</span><span class="sxs-lookup"><span data-stu-id="c9f95-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="c9f95-118">Khởi chạy Windows PowerShell trên máy mà sự cố xảy ra và chạy các lệnh sau:</span><span class="sxs-lookup"><span data-stu-id="c9f95-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="c9f95-119">Đính kèm tập tin vào trường hợp hỗ trợ của bạn.</span><span class="sxs-lookup"><span data-stu-id="c9f95-119">Attach the file to your support case.</span></span>
