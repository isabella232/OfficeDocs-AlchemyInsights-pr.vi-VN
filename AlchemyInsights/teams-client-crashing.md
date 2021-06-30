---
title: Teams máy khách gặp sự cố
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187743"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="b607a-102">Teams máy khách gặp sự cố</span><span class="sxs-lookup"><span data-stu-id="b607a-102">Teams client crashing</span></span>

<span data-ttu-id="b607a-103">Nếu máy khách Teams gặp sự cố, hãy thử cách sau:</span><span class="sxs-lookup"><span data-stu-id="b607a-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="b607a-104">Nếu bạn đang sử dụng ứng dụng Teams tính bàn, hãy [đảm bảo ứng dụng được cập nhật đầy đủ.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="b607a-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="b607a-105">Hãy đảm bảo rằng tất [cả các URL Microsoft 365 và dải địa chỉ đều](/microsoftteams/connectivity-issues) có thể truy nhập được.</span><span class="sxs-lookup"><span data-stu-id="b607a-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="b607a-106">Đăng nhập bằng tài khoản [](/office365/enterprise/view-service-health) người quản trị đối tượng thuê của bạn và kiểm tra Bảng điều khiển Tình trạng Dịch vụ của bạn để xác nhận rằng không tồn tại sự cố hoặc dịch vụ nào.</span><span class="sxs-lookup"><span data-stu-id="b607a-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="b607a-107">Gỡ cài đặt và cài đặt lại Teams Dụng</span><span class="sxs-lookup"><span data-stu-id="b607a-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="b607a-108">Duyệt đến thư mục %appdata%\Microsoft\Teams\ trên máy tính của bạn, rồi xóa tất cả các tệp trong thư mục đó.</span><span class="sxs-lookup"><span data-stu-id="b607a-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="b607a-109">Tải xuống và cài đặt [Ứng dụng Teams](https://www.microsoft.com/microsoft-teams/download-app)và nếu có thể, hãy cài đặt Teams với  tư cách người quản trị (bấm chuột phải vào chương trình cài đặt Teams, rồi chọn Chạy với tư cách người quản trị nếu có).</span><span class="sxs-lookup"><span data-stu-id="b607a-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="b607a-110">Nếu máy khách Teams gặp sự cố, hãy cố gắng tái tạo sự cố.</span><span class="sxs-lookup"><span data-stu-id="b607a-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="b607a-111">Nếu bạn có thể:</span><span class="sxs-lookup"><span data-stu-id="b607a-111">If you can:</span></span>

1. <span data-ttu-id="b607a-112">Sử dụng Trình ghi Bước để ghi lại các bước của bạn.</span><span class="sxs-lookup"><span data-stu-id="b607a-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="b607a-113">Đóng TẤT CẢ các ứng dụng không cần thiết hoặc bảo mật.</span><span class="sxs-lookup"><span data-stu-id="b607a-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="b607a-114">Khởi chạy Trình ghi Bước và tái tạo sự cố khi đăng nhập bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="b607a-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="b607a-115">[Thu thập nhật ký nhóm ghi lại các bước tiến hành lại được ghi lại.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="b607a-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="b607a-116">**Lưu** ý : Đảm bảo bạn ghi lại được địa chỉ đăng nhập của người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="b607a-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="b607a-117">Thu thập thông tin kết xuất và/hoặc Bộ chứa lỗi (Windows).</span><span class="sxs-lookup"><span data-stu-id="b607a-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="b607a-118">Khởi Windows Powershell trên máy đang xảy ra sự cố và chạy các lệnh sau (sau mỗi lệnh, hãy nhấn Enter):</span><span class="sxs-lookup"><span data-stu-id="b607a-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="b607a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="b607a-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="b607a-120">Sau khi tạo tệp văn bản và xuất hiện trên màn hình của bạn, hãy lưu tệp và đính kèm tệp vào yêu cầu dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="b607a-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
