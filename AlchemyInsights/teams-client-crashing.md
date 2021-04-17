---
title: Các nhóm khách hàng bị rơi?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826293"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="cf1c5-102">Các nhóm khách hàng bị rơi?</span><span class="sxs-lookup"><span data-stu-id="cf1c5-102">Teams client crashing?</span></span>

<span data-ttu-id="cf1c5-103">Nếu máy khách nhóm của bạn bị rơi, hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="cf1c5-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="cf1c5-104">Nếu bạn đang sử dụng ứng dụng nhóm màn hình nền, [hãy đảm bảo rằng ứng dụng đã được cập nhật đầy đủ](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="cf1c5-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="cf1c5-105">Hãy đảm bảo rằng tất cả các [URL và dải địa chỉ của Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) đều có thể truy nhập.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="cf1c5-106">Đăng nhập bằng tài khoản người quản trị đối tượng thuê của bạn và kiểm tra bảng điều khiển trạng thái [dịch vụ](https://docs.microsoft.com/office365/enterprise/view-service-health) của bạn để xác minh rằng không có sự suy thoái về mất hoặc bị mất</span><span class="sxs-lookup"><span data-stu-id="cf1c5-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="cf1c5-107">Gỡ cài đặt và cài đặt lại ứng dụng nhóm (liên kết)</span><span class="sxs-lookup"><span data-stu-id="cf1c5-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="cf1c5-108">Duyệt đến%appdata%\Microsoft\teams\ thư mục trên máy tính của bạn và xóa tất cả các tệp trong thư mục đó.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="cf1c5-109">[Tải xuống và cài đặt ứng dụng nhóm](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)và nếu có thể, hãy cài đặt các nhóm làm người quản trị (bấm chuột phải vào trình cài đặt nhóm, rồi chọn "chạy với tư việc là người quản trị" nếu có).</span><span class="sxs-lookup"><span data-stu-id="cf1c5-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="cf1c5-110">Nếu máy khách nhóm của bạn vẫn gặp phải, bạn có thể tái tạo vấn đề này không?</span><span class="sxs-lookup"><span data-stu-id="cf1c5-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="cf1c5-111">Nếu vậy:</span><span class="sxs-lookup"><span data-stu-id="cf1c5-111">If so:</span></span>

1. <span data-ttu-id="cf1c5-112">Sử dụng trình ghi bước để nắm bắt các bước của bạn.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="cf1c5-113">Đóng tất cả các ứng dụng không cần thiết hoặc bảo mật.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="cf1c5-114">Khởi động các bước ghi âm và tái tạo vấn đề trong khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="cf1c5-115">[Thu thập Nhật ký nhóm chụp các bước đã ghi Repro](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="cf1c5-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="cf1c5-116">**Lưu ý**: Hãy đảm bảo rằng bạn đã nắm bắt địa chỉ đăng nhập của người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="cf1c5-117">Thu thập thông tin thùng chứa và/hoặc lỗi (Windows).</span><span class="sxs-lookup"><span data-stu-id="cf1c5-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="cf1c5-118">Khởi chạy Windows PowerShell trên máy tính có sự cố xảy ra và chạy các lệnh sau đây:</span><span class="sxs-lookup"><span data-stu-id="cf1c5-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="cf1c5-119">Đính kèm tệp vào trường hợp hỗ trợ của bạn.</span><span class="sxs-lookup"><span data-stu-id="cf1c5-119">Attach the file to your support case.</span></span>
